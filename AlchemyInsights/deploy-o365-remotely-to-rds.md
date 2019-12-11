---
title: Déploiement d’Office 365 ProPlus pour une utilisation partagée sur RDS, Terminal Server ou VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959458"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Déploiement d’Office 365 ProPlus pour une utilisation partagée sur RDS, Terminal Server ou VDI

Pour déployer Office 365 ProPlus à l’aide des services Bureau à distance (RDS), anciennement services Terminal Server :
- Vous devez disposer d’un plan Microsoft 365 for Business ou d’un plan Office 365 incluant Office 365 ProPlus, comme Office 365 entreprise E3 ou entreprise E5.
   > [!NOTE] 
   > Les plans Office 365 Business et Office 365 Business Premium n’incluent pas Office 365 ProPlus.
- Vous devez activer [l’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Vous pouvez également télécharger et exécuter l' [Assistant support et récupération Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pour installer Office 365 ProPlus en mode d’activation d’ordinateur partagé.

Pour plus d’informations sur les conditions préalables, les instructions de configuration et des conseils sur les installations personnalisées à l’aide de l’outil déploiement d’Office, consultez la rubrique [Deploy office 365 ProPlus à l’aide des services Bureau à distance](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Pour corriger les erreurs liées à l’activation d’ordinateurs partagés :
- Voir [résoudre les problèmes liés à l’activation d’ordinateurs partagés pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Voir [Réinitialiser l’état d’activation d’Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Si vous souhaitez installer Office 365 ProPlus sur RDS à partir du centre d’administration de Microsoft 365, ***qui utilise les paramètres d’installation par défaut***, procédez comme suit :

1.  Consultez la planification d’Office 365. [Découvrir comment](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Si nécessaire, passez à une autre offre Office 365. [Découvrir comment](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Si Office est déjà installé sur le serveur RDS à l’aide d’autres plans Office 365, désinstallez-le. Par exemple, en accédant à **panneau de configuration** > **désinstaller un programme**. Désinstallation à l’aide [de l’Assistant support et récupération Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous rencontrez des problèmes.
4.  Sur le serveur RDS, connectez-vous au centre d’administration Microsoft 365 avec votre compte d’administrateur et [installez Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Une fois Office installé, ***ne pas ouvrir ou se connecter*** à une application Office.
6.  Sur le serveur RDS, activez l’activation d’ordinateurs partagés en modifiant le registre en procédant comme suit :
   1. Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran et sélectionnez **exécuter**. Dans la zone Ouvrir, tapez **regedit**, puis cliquez sur **OK**.
   2. Sélectionnez **Oui** lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.
   3. Dans l’éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec un paramètre de 1 sous HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.
   4. Sur le serveur RDS, ***Connectez-vous en tant qu’utilisateur final*** et [Vérifiez que l’activation d’ordinateurs partagés est activée pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

