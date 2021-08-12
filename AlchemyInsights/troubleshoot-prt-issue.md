---
title: Résoudre le problème d’prt
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972714"
---
# <a name="troubleshoot-prt-issue"></a>Résoudre le problème d’prt

Pour que tout appareil termine l’authentification, il doit être entièrement inscrit et en bon état et en mesure d’acquérir un jeton d’actualisation principal (PRT).

Le processus hybride d’inscription à la jointation Azure AD nécessite que les appareils soient sur un réseau d’entreprise. Il fonctionne également sur VPN, mais il existe des avertissements à ce qui se fait. Nous avons entendu les clients qui ont besoin d’aide pour résoudre les problèmes du processus hybride d’inscription à Azure AD dans des circonstances de travail à distance. Voici une répartition de ce qui se passe « sous le capot » pendant le processus d’inscription.

**Environnement d’authentification cloud (à l’aide de la synchronisation de hachage de mot de passe Azure AD ou de l’authentification directe)**

Ce flux d’inscription est également appelé « synchronisation de joints ».

1. Windows 10 un enregistrement SCP lorsque l’utilisateur se connecte à l’appareil.
    1. L’appareil tente d’abord de récupérer les informations client du point de service côté client dans le Registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. En cas d’échec, l’appareil communique avec Active Directory (AD) local pour obtenir des informations client à partir du point de connexion de service (SCP). Pour vérifier le protocole SCP, reportez-vous à ce [document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Nous vous recommandons d’activer SCP dans AD et d’utiliser uniquement le point de contrôle de service côté client pour la validation initiale.

2. Windows 10 tente de communiquer avec Azure AD dans le contexte système pour s’authentifier auprès d’Azure AD. Vous pouvez vérifier si l’appareil peut accéder aux ressources Microsoft sous le compte système à l’aide du script Test Device Registration Connectivity.

3. Windows 10 génère un certificat auto-signé et le stocke sous l’objet ordinateur dans AD local. Cela nécessite une vision d’accès au contrôleur de domaine.

4. Un objet appareil qui possède un certificat est synchronisé avec Azure AD via Azure AD Connecter. Le cycle de synchronisation est toutes les 30 minutes par défaut, mais il dépend de la configuration d’Azure AD Connecter. Pour plus d’informations, reportez-vous à ce [document.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. À ce stade, vous devriez être en mesure de voir l’appareil objet dans l’état « En attente » sous le portail Azure.

6. Lors de la prochaine connexion de l’Windows 10, l’inscription est terminée. 

> [!NOTE]
> Si vous utilisez un VPN et qu’un processus de connexion par ouverture de session met fin à la connectivité de domaine, vous pouvez déclencher l’inscription manuellement :
 1. Émettre un dsregcmd /join localement à l’invite de l’administrateur ou à distance via PSExec sur votre PC. Par exemple, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Pour plus d’informations sur les problèmes de jointisation hybride, voir [Résoudre les problèmes d’appareils.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
