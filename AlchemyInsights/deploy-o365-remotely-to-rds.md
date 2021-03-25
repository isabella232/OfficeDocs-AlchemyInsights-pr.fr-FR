---
title: Déploiement de Microsoft 365 Apps pour entreprise pour une utilisation partagée sur RDS, Terminal Server ou VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200671"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Déploiement de Microsoft 365 Apps pour entreprise pour une utilisation partagée sur RDS, Terminal Server ou VDI

Pour déployer Microsoft 365 Apps for enterprise à l’aide des services Bureau à distance (RDS), anciennement nommés Services Terminal Services :

- Vous devez avoir une offre Microsoft 365 Entreprise ou Une offre Office 365 qui inclut Microsoft 365 Apps for enterprise, telle qu’Office 365 Entreprise E3 ou Entreprise E5.
   > [!NOTE]
   > Les plans Microsoft 365 Apps for business et Microsoft 365 Business Standard n’incluent pas les applications Microsoft 365 pour les entreprises.
- Vous devez activer [l’activation d’ordinateurs partagés.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Vous pouvez également télécharger et exécuter [l’Assistant Support](https://aka.ms/SaRA_OfficeSCA_M365Portal) et récupération Microsoft pour installer Microsoft 365 Apps for enterprise en mode d’activation d’ordinateurs partagés.

Pour plus d’informations sur les conditions préalables, les instructions d’installation et les instructions sur les installations personnalisées à l’aide de l’outil Déploiement d’Office, voir [Déployer Microsoft 365 Apps pour](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)entreprise à l’aide des services Bureau à distance.

Pour corriger les erreurs liées à l’activation d’ordinateurs partagés :

- Voir Résoudre les problèmes d’activation d’ordinateurs [partagés pour Microsoft 365 Apps for enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Voir [Réinitialiser les applications Microsoft 365 pour l’état d’activation d’entreprise](https://go.microsoft.com/fwlink/?linkid=2109218).

Si vous souhaitez installer Microsoft 365 Apps for enterprise sur RDS à partir du Centre d’administration Microsoft 365, qui utilise les paramètres d’installation par défaut, utilisez les ***étapes suivantes***:

1. Vérifiez l’abonnement que vous avez. [Découvrir comment](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Si nécessaire, passez à un autre abonnement. [Découvrir comment](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Si Office est déjà installé sur le serveur RDS à l’aide d’autres abonnements Microsoft, désinstallez-le. Par exemple, en allant dans le **Panneau de contrôle**  >  **Désinstaller un programme**. Désinstallez-vous à l’aide de [l’Assistant Support et](https://aka.ms/SARA-OfficeUninstall-Alchemy) récupération Microsoft si vous êtes en train de faire des problèmes.
4. Sur le serveur RDS, connectez-vous au Centre d’administration Microsoft 365 avec votre compte d’administrateur et installez [Microsoft 365 Apps pour entreprise.](https://portal.office.com/OLS/MySoftware.aspx)
5. Une fois Office installé, ne vous ouvrez pas ou ne ***vous connectez à*** aucune application Office.
6. Sur le serveur RDS, activez l’activation d’ordinateurs partagés en éditant le Registre en suivant les étapes suivantes :
   1. Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran, puis sélectionnez **Exécuter.** Dans la zone Ouvrir, tapez **regedit** puis cliquez sur **OK**.
   2. Sélectionnez **Oui** lorsque vous y invitez l’Éditeur du Registre pour apporter des modifications à votre appareil.
   3. Dans l’Éditeur du Registre, ajoutez une valeur de chaîne **sharedComputerLicensing** avec le paramètre 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Sur le serveur ***RDS,*** connectez-vous en tant qu’utilisateur final et vérifiez que l’activation d’ordinateurs partagés est activée pour [Microsoft 365 Apps pour entreprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
