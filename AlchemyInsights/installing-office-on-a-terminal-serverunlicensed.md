---
title: Installation d’Office sur un serveur Terminal Server sans licence
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205407"
---
# <a name="installing-office-on-a-terminal-server"></a>Installation d’Office sur un serveur Terminal Server

Pour déployer Office 365 ProPlus sur un serveur Windows à l’aide des services Bureau à distance (RDS), anciennement services Terminal Server :
  
- Vous devez disposer d’un plan Office 365 qui inclut Office 365 ProPlus, comme Office 365 entreprise E3 ou entreprise E5. Les plans Office 365 Business et Office 365 Business Premium n’incluent pas Office 365 ProPlus.

- Vous devez activer [l’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Si vous souhaitez installer Office 365 ProPlus sur RDS à partir du centre d’administration de Microsoft 365, ***qui utilise les paramètres d’installation par défaut***, procédez comme suit.

> [!TIP]
> Vous pouvez également télécharger et exécuter l' [Assistant support et récupération Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pour installer Office 365 ProPlus en mode d’activation d’ordinateur partagé.
  
1. Consultez la planification d’Office 365. [Découvrez comment](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Si nécessaire, passez à une autre offre Office 365. [Découvrez comment](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Si Office est déjà installé sur le serveur RDS à l’aide d’autres plans Office 365, désinstallez-le. Par exemple, en accédant à panneau \> de configuration désinstaller un programme. Désinstallation à l’aide [de l’Assistant support et récupération Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous rencontrez des problèmes.

4. Sur le serveur RDS, connectez-vous au centre d’administration Microsoft 365 avec votre compte d’administrateur et [installez Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Une fois Office installé, ***ne pas ouvrir ou se connecter*** à une application Office.

6. Sur le serveur RDS, activez l’activation d’ordinateurs partagés en modifiant le registre en procédant comme suit :

1. Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran et sélectionnez Exécuter. Dans la zone Ouvrir, tapez **regedit**, puis cliquez sur OK.

2. Sélectionnez Oui lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.

3. Dans l’éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec un paramètre de 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Sur le serveur RDS, ***Connectez-vous en tant qu’utilisateur final*** et [Vérifiez que l’activation d’ordinateurs partagés est activée pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Pour plus d’informations sur les conditions préalables, les instructions de configuration et des conseils sur les installations personnalisées à l’aide de l’outil déploiement d’Office, consultez la rubrique [Deploy office 365 ProPlus à l’aide des services Bureau à distance](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Pour résoudre les erreurs liées à l’activation d’ordinateurs partagés, voir [résoudre les problèmes liés à l’activation d’ordinateurs partagés pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  