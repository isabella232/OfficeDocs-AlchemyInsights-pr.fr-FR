---
title: Installation d’Office sur un serveur Terminal Server sans licence
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663115"
---
# <a name="installing-office-on-a-terminal-server"></a>Installation d’Office sur un serveur Terminal Server

Pour déployer des applications Microsoft 365 pour Enterprise sur un serveur Windows à l’aide des services Bureau à distance (RDS), anciennement services Terminal Server :
  
- Vous devez disposer d’un abonnement Microsoft 365 qui inclut les applications Microsoft 365 pour les entreprises, comme Office 365 entreprise E3 ou entreprise E5. Les applications Microsoft 365 Apps for Business et Microsoft 365 pour les offres Business Premium n’incluent pas les applications Microsoft 365 pour les entreprises.

- Vous devez activer [l’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Si vous souhaitez installer Microsoft 365 apps pour Enterprise sur RDS à partir du centre d’administration de Microsoft 365, ***qui utilise les paramètres d’installation par défaut***, procédez comme suit.

> [!TIP]
> Vous pouvez également télécharger et exécuter l' [Assistant support et récupération Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pour installer les applications Microsoft 365 pour Enterprise en mode d’activation d’ordinateur partagé.
  
1. Vérifiez l’abonnement Microsoft 365 que vous avez. [Découvrez comment](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Si nécessaire, passez à un autre abonnement Microsoft 365. [Découvrez comment](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Si Office est déjà installé sur le serveur RDS à l’aide d’autres abonnements Microsoft 365, désinstallez-le. Par exemple, en accédant à panneau de configuration \> désinstaller un programme. Désinstallation à l’aide [de l’Assistant support et récupération Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous rencontrez des problèmes.

4. Sur le serveur RDS, connectez-vous au centre d’administration Microsoft 365 avec votre compte d’administrateur et [Installez microsoft 365 apps pour entreprises](https://portal.office.com/OLS/MySoftware.aspx).

5. Une fois Office installé, ***ne pas ouvrir ou se connecter*** à une application Office.

6. Sur le serveur RDS, activez l’activation d’ordinateurs partagés en modifiant le registre en procédant comme suit :

1. Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran et sélectionnez Exécuter. Dans la zone Ouvrir, tapez **regedit**, puis cliquez sur OK.

2. Sélectionnez Oui lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.

3. Dans l’éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec un paramètre de 1 sous HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.

7. Sur le serveur RDS, ***Connectez-vous en tant qu’utilisateur final*** et [Vérifiez que l’activation d’ordinateurs partagés est activée pour les applications Microsoft 365 pour entreprises](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Pour plus d’informations sur les conditions préalables, les instructions de configuration et des conseils sur les installations personnalisées à l’aide de l’outil déploiement d’Office, consultez la rubrique [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Pour résoudre les erreurs liées à l’activation d’ordinateurs partagés, consultez la rubrique [Troubleshoot Problems with Shared Computer activation for Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  