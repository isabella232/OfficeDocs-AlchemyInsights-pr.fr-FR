---
title: Déploiement d’applications Microsoft 365 pour Enterprise pour une utilisation partagée sur RDS, Terminal Server ou VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704703"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Déploiement d’applications Microsoft 365 pour Enterprise pour une utilisation partagée sur RDS, Terminal Server ou VDI

Pour déployer des applications Microsoft 365 pour Enterprise à l’aide des services Bureau à distance (RDS), anciennement services Terminal Server :
- Vous devez disposer d’un plan Microsoft 365 pour les entreprises ou d’un plan Office 365 incluant les applications Microsoft 365 pour entreprises, telles qu’Office 365 entreprise E3 ou entreprise E5.
   > [!NOTE] 
   > Les plans Microsoft 365 Apps for Business et Microsoft 365 Business Premium standard n’incluent pas les applications Microsoft 365 pour les entreprises.
- Vous devez activer [l’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Vous pouvez également télécharger et exécuter l' [Assistant support et récupération Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pour installer les applications Microsoft 365 pour Enterprise en mode d’activation d’ordinateur partagé.

Pour plus d’informations sur les conditions préalables, les instructions de configuration et des conseils sur les installations personnalisées à l’aide de l’outil déploiement d’Office, consultez la rubrique [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Pour corriger les erreurs liées à l’activation d’ordinateurs partagés :
- Voir [résoudre les problèmes liés à l’activation d’ordinateurs partagés pour les applications Microsoft 365 pour les entreprises](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Voir [Réinitialiser les applications Microsoft 365 pour l’état d’activation d’entreprise](https://go.microsoft.com/fwlink/?linkid=2109218).

Si vous souhaitez installer Microsoft 365 apps pour Enterprise sur RDS à partir du centre d’administration de Microsoft 365, ***qui utilise les paramètres d’installation par défaut***, procédez comme suit :

1.    Vérifiez l’abonnement dont vous disposez. [Découvrir comment](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Si nécessaire, basculez vers un autre abonnement. [Découvrir comment](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Si Office est déjà installé sur le serveur RDS à l’aide d’autres abonnements Microsoft, désinstallez-le. Par exemple, en accédant à **panneau de configuration** > **désinstaller un programme**. Désinstallation à l’aide [de l’Assistant support et récupération Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous rencontrez des problèmes.
4.    Sur le serveur RDS, connectez-vous au centre d’administration Microsoft 365 avec votre compte d’administrateur et [Installez microsoft 365 apps pour entreprises](https://portal.office.com/OLS/MySoftware.aspx).
5.    Une fois Office installé, ***ne pas ouvrir ou se connecter*** à une application Office.
6.    Sur le serveur RDS, activez l’activation d’ordinateurs partagés en modifiant le registre en procédant comme suit :
   1. Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran et sélectionnez **exécuter**. Dans la zone Ouvrir, tapez **regedit**, puis cliquez sur **OK**.
   2. Sélectionnez **Oui** lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.
   3. Dans l’éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec un paramètre de 1 sous HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.
   4. Sur le serveur RDS, ***Connectez-vous en tant qu’utilisateur final*** et [Vérifiez que l’activation d’ordinateurs partagés est activée pour les applications Microsoft 365 pour entreprises](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

