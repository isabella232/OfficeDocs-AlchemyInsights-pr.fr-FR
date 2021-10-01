---
title: Déploiement de Microsoft 365 Apps pour une utilisation partagée sur RDS, Terminal Server ou VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077248"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Déploiement de Microsoft 365 Apps pour une utilisation partagée sur RDS, Terminal Server ou VDI

Pour déployer Microsoft 365 Apps à l’aide des services Bureau à distance (RDS), anciennement services Terminal Services, vous devez :

- Utilisez le correctif simple pour activer TLS 1.2 par défaut si vous exécutez une version antérieure de Windows (par exemple, Windows 7 SP1, Windows Server 2008 R2). Pour obtenir des correctifs simples et plus d’informations, voir Mise à jour pour activer [TLS 1.1 et TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)en tant que protocoles sécurisés par défaut dans WinHTTP dans Windows . 
- Avoir un plan qui inclut Applications Microsoft 365 pour les grandes entreprises (précédemment Office 365 Plus). Par exemple, Office 365 E3 ou Microsoft 365 E5, ou tout plan qui inclut la version de bureau de Project ou de Visio, telle que Project (plan 3) ou Visio (plan 2), ou le plan Microsoft 365 Business Premium, qui inclut également Applications Microsoft 365 pour les PME.
- Activer l’activation d’ordinateurs partagés. Pour plus d’informations, voir [Vue d’ensemble de l’activation d’ordinateurs Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Remarque**: pour installer les Microsoft 365 Apps en mode d’activation d’ordinateurs partagés, téléchargez et exécutez [l’application Microsoft Assistant Support et récupération](https://aka.ms/SaRA_OfficeSCA_M365Portal). Pour plus d’informations sur les conditions préalables, les instructions de configuration et les instructions de personnalisation des installations à l’aide de l’outil déploiement Office, voir [Déployer Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)à l’aide des services Bureau à distance.

Pour corriger les erreurs liées à l’activation d’ordinateurs partagés, voir :

- [Résoudre les problèmes d’activation d’ordinateurs partagés pour Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Réinitialiser l’état d’activation de Microsoft 365 Apps for enterprise](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Si vous souhaitez installer Microsoft 365 Apps sur RDS à partir du Centre d'administration Microsoft 365, qui utilise les paramètres d’installation par défaut, suivez les étapes suivantes :

1. Vérifiez le Microsoft 365 votre plan. Pour plus d’informations, [voir de quel abonnement ai-je ?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Si nécessaire, basculez vers une autre Microsoft 365 plan. Pour plus d’informations, [voir Mettre à niveau vers un autre plan.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Si Microsoft 365 Apps est déjà installé sur le serveur RDS à l’aide d’autres plans incompatibles, désinstallez-le en allant dans le Panneau de commande  >  **Désinstaller un programme.** Si vous avez des problèmes, désinstallez-le en téléchargeant [Microsoft Assistant Support et récupération](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Sur le serveur RDS, connectez-vous au Centre d'administration Microsoft 365 avec votre compte d’administrateur et [installez Office](https://portal.office.com/OLS/MySoftware.aspx).

   Une fois Office installé, ne vous ouvrez pas ou ne connectez-vous à aucune application Office applications.

1. Sur le serveur RDS, activez l’activation d’ordinateurs partagés en éditant le Registre :

   1. Cliquez avec le bouton droit Windows dans le coin inférieur gauche de votre écran, puis sélectionnez **Exécuter.** Dans la zone Ouvrir, tapez **regedit** puis cliquez sur **OK**.

   1. Lorsque vous y invitez l’Éditeur du Registre à apporter des modifications à votre appareil, sélectionnez **Oui**.

   1. Dans l’Éditeur du Registre, sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, ajoutez une valeur de chaîne **SharedComputerLicensing** avec le paramètre **1** .

1. Sur le serveur RDS, connectez-vous en tant qu’utilisateur final et vérifiez que l’activation d’ordinateurs partagés est activée pour Microsoft 365 Apps. 

   Pour plus d’informations, [voir Vérifier que l’activation](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)d’ordinateurs partagés est activée pour Microsoft 365 Apps .