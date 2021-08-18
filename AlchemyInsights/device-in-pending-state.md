---
title: Appareil en attente
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
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330370"
---
# <a name="device-in-pending-state"></a>Appareil en attente

**Conditions préalables :**

1. Si vous êtes en train de définir des inscriptions d’appareils pour la première fois, assurez-vous que vous avez examiné l’introduction à la gestion des appareils dans [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) qui vous guidera sur la façon d’obtenir des appareils sous le contrôle d’Azure AD.
2. Si vous inscrivez des appareils directement dans Azure AD et que vous les inscrivez dans Intune, vous [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) devez vous assurer que vous avez configuré [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) et que la licence est en place en premier.
3. Assurez-vous que vous êtes autorisé à effectuer des opérations dans Azure AD et dans AD local. Seul un administrateur général dans Azure AD peut gérer les paramètres d’enregistrement des appareils. Par ailleurs, si vous configurez les enregistrements automatiques dans votre Active Directory local, vous devez être administrateur d’Active Directory et des services ADFS (le cas échéant).

Le processus hybride d’inscription à la jointation Azure AD nécessite que les appareils soient sur le réseau d’entreprise. Il fonctionne également sur VPN, mais il existe quelques avertissements à ce à ce jour. Nous avons entendu les clients qui ont besoin d’aide pour résoudre les problèmes du processus d’inscription hybride à Azure AD dans des circonstances de travail à distance.

**Environnement d’authentification cloud (à l’aide de la synchronisation de hachage de mot de passe Azure AD ou de l’authentification directe)**

Ce flux d’inscription est également appelé « synchronisation de joints ».

Voici une répartition de ce qui se produit pendant le processus d’inscription :

1. Windows 10 l’enregistrement SCP (Service Connection Point) lorsque l’utilisateur se connecte à l’appareil.

    1. L’appareil tente d’abord de récupérer des informations client à partir du point de service SCP côté client dans le Registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pour plus d’informations, voir [le document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. En cas d’échec, l’appareil communique avec Active Directory local pour obtenir des informations sur le client auprès de SCP. Pour vérifier SCP, reportez-vous à [ce document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Remarque**: nous vous recommandons d’activer SCP dans Active Directory et d’utiliser uniquement le point de contrôle de service côté client pour la validation initiale.

2. Windows 10 tente de communiquer avec Azure AD dans le contexte système pour s’authentifier auprès d’Azure AD.

    Vous pouvez vérifier si l’appareil peut accéder aux ressources Microsoft sous le compte système à l’aide du [script Test Device Registration Connectivity](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 génère un certificat auto-signé et le stocke sous l’objet ordinateur dans Active Directory local. Cela nécessite une vision d’accès au contrôleur de domaine.

4. L’objet appareil qui possède un certificat est synchronisé avec Azure AD via Azure AD Connecter. Le cycle de synchronisation est toutes les 30 minutes par défaut, mais il dépend de la configuration d’Azure AD Connecter. Pour plus d’informations, reportez-vous à [ce document.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. À ce stade, vous devriez être en mesure de voir l’appareil objet dans l’état «**En** attente » sous le blade device du portail Azure.

6. Lors de la prochaine connexion de l’Windows 10, l’inscription est terminée.

    **Remarque**: si vous utilisez un VPN et que la connexion/la connexion met fin à la connectivité de domaine, vous pouvez déclencher l’inscription manuellement. Pour cela :
    
    Émettre `dsregcmd /join` une invite d’administration localement ou à distance via PSExec sur votre PC.\
    Par exemple : `PsExec -s \\win10client01 cmd, dsregcmd /join`

Pour les problèmes courants d’Azure Active Directory’inscription des appareils, voir [FAQ sur les appareils.](https://docs.microsoft.com/azure/active-directory/devices/faq)
