---
title: Résoudre les problèmes liés à PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571876"
---
# <a name="troubleshoot-prt-issue"></a>Résoudre les problèmes liés à PRT

Pour que tout appareil s’exécute authentifié, il doit être entièrement enregistré et en parfait état et capable d’acquérir un jeton d’actualisation principal (PRT).

Le processus d’inscription de jointure Azure AD hybride nécessite que les appareils soient sur un réseau d’entreprise. Il fonctionne également sur VPN, mais il existe quelques inconvénients à ce propos. Nous avons entendu des clients qui ont besoin d’aide pour résoudre les problèmes liés au processus d’inscription de participation à Azure AD hybride dans des conditions de travail à distance. Voici une ventilation de ce qui se passe « en coulisse » pendant le processus d’inscription.

**Environnement d’authentification Cloud (à l’aide de l’authentification directe ou de synchronisation de hachage de mot de passe Azure AD)**

Ce flux d’enregistrement est également appelé « jointure de synchronisation ».

1. Windows 10 identifie un enregistrement SCP lorsque l’utilisateur se connecte à l’appareil.
    1. Le périphérique tente d’abord de récupérer les informations client à partir du SCP côté client dans le registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pour plus d’informations, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. En cas d’échec, le périphérique communique avec Active Directory local (AD) pour obtenir les informations du client à partir du point de connexion de service (SCP). Pour vérifier le SCP, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Nous vous recommandons d’activer SCP dans AD et de n’utiliser que le SCP côté client pour la validation initiale.

2. Windows 10 tente de communiquer avec Azure AD dans le contexte système pour s’authentifier auprès d’Azure AD. Vous pouvez vérifier si l’appareil peut accéder aux ressources Microsoft sous le compte système à l’aide du script de test de connectivité de Device Registration.

3. Windows 10 génère un certificat auto-signé et le stocke sous l’objet ordinateur dans AD locale. Cela nécessite une visibilité du contrôleur de domaine.

4. Un objet périphérique qui a un certificat est synchronisé avec Azure AD via Azure AD Connect. Le cycle de synchronisation est défini toutes les 30 minutes par défaut, mais dépend de la configuration d’Azure AD Connect. Pour plus d’informations, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. À ce stade, vous devriez être en mesure d’afficher l’objet de l’objet dans l’État « en attente » sous Blade de périphérique d’Azure Portal.

6. Lors de la connexion utilisateur suivante à Windows 10, l’inscription est effectuée. 

> [!NOTE]
> Si vous êtes sur un VPN et qu’un processus de fermeture de session ferme le domaine, vous pouvez déclencher l’inscription manuellement :
 1. Émettez une invite dsregcmd/Join localement sur l’administrateur ou à distance via PSExec à votre PC. Par exemple, PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Pour plus d’informations sur les problèmes de jointure hybride, consultez la rubrique [Troubleshoot Devices](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)problem.
