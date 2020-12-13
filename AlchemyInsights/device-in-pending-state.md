---
title: Appareil en état d’attente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652191"
---
# <a name="device-in-pending-state"></a>Appareil en état d’attente

**Conditions préalables**

1. Si vous configurez les inscriptions d’appareils pour la première fois, vérifiez que vous avez lu la rubrique relative à la gestion des appareils [dans Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) pour vous aider à obtenir des périphériques sous le contrôle d’Azure ad.
2. Si vous enregistrez les appareils dans Azure AD directement et en les inscrivant dans Intune, vous devez vous assurer que vous avez [configuré Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) et que la gestion des [licences](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) est en place.
3. Assurez-vous que vous êtes autorisé à effectuer des opérations dans Azure AD et AD sur site. Seul un administrateur général dans Azure AD peut gérer les paramètres des inscriptions d’appareils. En outre, si vous configurez des enregistrements automatiques dans votre annuaire Active Directory local, vous devez être un administrateur d’Active Directory et d’AD FS (le cas échéant).

Le processus d’inscription hybride Azure AD requiert des périphériques sur le réseau d’entreprise. Il fonctionne également sur VPN, mais il existe quelques inconvénients à ce propos. Nous avons entendu des clients qui ont besoin d’aide pour résoudre les problèmes liés au processus d’inscription hybride Azure AD dans des conditions de travail à distance.

**Environnement d’authentification Cloud (à l’aide de l’authentification directe ou de synchronisation de hachage de mot de passe Azure AD)**

Ce flux d’enregistrement est également appelé « jointure de synchronisation ».

Voici une répartition de ce qui se produit pendant le processus d’inscription :

1. Windows 10 identifie l’enregistrement du point de connexion de service (SCP) lorsque l’utilisateur se connecte à l’appareil.

    1. Le périphérique tente d’abord de récupérer les informations client à partir du SCP côté client dans le registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pour plus d’informations, consultez la rubrique [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. En cas d’échec, le périphérique communique avec Active Directory local pour obtenir les informations du client auprès du SCP. Pour vérifier le SCP, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Nous vous recommandons d’activer SCP dans Active Directory et de n’utiliser que le SCP côté client pour la validation initiale.

2. Windows 10 tente de communiquer avec Azure AD dans le contexte système pour s’authentifier auprès d’Azure AD.

    Vous pouvez vérifier si l’appareil peut accéder aux ressources Microsoft sous le compte système à l’aide du [script de test de connectivité de Device Registration](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 génère un certificat auto-signé et le stocke sous l’objet ordinateur dans Active Directory en local. Cela nécessite une visibilité du contrôleur de domaine.

4. L’objet appareil dont le certificat est synchronisé est synchronisé avec Azure AD via Azure AD Connect. Le cycle de synchronisation est défini toutes les 30 minutes par défaut, mais dépend de la configuration d’Azure AD Connect. Pour plus d’informations, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. À ce stade, vous devriez être en mesure d’afficher l’objet de l’objet dans l’état «**en attente**» sous Blade de périphérique d’Azure Portal.

6. Lors de la connexion utilisateur suivante à Windows 10, l’inscription est effectuée.

    > [!NOTE]
    > Si vous êtes sur un VPN et que la déconnexion et la connexion se terminent, vous pouvez déclencher l’inscription manuellement. Pour cela :
    >
    > Émettez une `dsregcmd /join` invite locale sur l’administrateur ou à distance via PsExec à votre PC.
    >
    > Par exemple : `PsExec -s \\win10client01 cmd, dsregcmd /join`

Pour les problèmes courants liés à l’inscription d’appareils Azure Active Directory, consultez la rubrique [périphériques FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).
