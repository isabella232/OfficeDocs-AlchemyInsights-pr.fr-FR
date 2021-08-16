---
title: Déploiement de Applications Microsoft 365 pour les grandes entreprises pour une utilisation partagée sur RDS, Terminal Server ou VDI
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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031476"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Déploiement de Applications Microsoft 365 pour les grandes entreprises pour une utilisation partagée sur RDS, Terminal Server ou VDI

Pour déployer Applications Microsoft 365 pour les grandes entreprises à l’aide des services Bureau à distance (RDS), anciennement nommés Services Terminal Services :

- Vous devez avoir une offre Microsoft 365 Entreprise ou une offre Office 365 qui inclut des Applications Microsoft 365 pour les grandes entreprises, telles que Office 365 Entreprise E3 ou Enterprise E5.
   > [!NOTE]
   > Les plans Applications Microsoft 365 pour les PME et Microsoft 365 Business Standard ne comprennent pas de Applications Microsoft 365 pour les grandes entreprises.
- Vous devez activer [l’activation d’ordinateurs partagés.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Vous pouvez également télécharger et exécuter [microsoft Assistant Support et récupération](https://aka.ms/SaRA_OfficeSCA_M365Portal) pour installer Applications Microsoft 365 pour les grandes entreprises en mode d’activation d’ordinateurs partagés.

Pour plus d’informations sur les conditions préalables, les instructions d’installation et les instructions sur les installations personnalisées à l’aide de l’outil déploiement Office, voir [Déployer Applications Microsoft 365 pour les grandes entreprises](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)à l’aide des services Bureau à distance.

Pour corriger les erreurs liées à l’activation d’ordinateurs partagés :

- Voir [Résoudre les problèmes d’activation d’ordinateurs partagés pour Applications Microsoft 365 pour les grandes entreprises](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Voir [Réinitialiser les applications Microsoft 365 pour l’état d’activation d’entreprise](https://go.microsoft.com/fwlink/?linkid=2109218).

Si vous souhaitez installer Applications Microsoft 365 pour les grandes entreprises sur RDS à partir du Centre d’administration Microsoft 365, qui utilise les ***paramètres d’installation*** par défaut, utilisez les étapes suivantes :

1. Vérifiez l’abonnement que vous avez. [Découvrir comment](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Si nécessaire, passez à un autre abonnement. [Découvrir comment](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Si Office est déjà installé sur le serveur RDS à l’aide d’autres abonnements Microsoft, désinstallez-le. Par exemple, en allant dans le **Panneau de contrôle**  >  **Désinstaller un programme**. Désinstallez [à l’Assistant Support et récupération](https://aka.ms/SARA-OfficeUninstall-Alchemy) microsoft si vous êtes en train de faire des problèmes.
4. Sur le serveur RDS, connectez-vous au Centre d’administration Microsoft 365 avec votre compte d’administrateur et [installez Applications Microsoft 365 pour les grandes entreprises](https://portal.office.com/OLS/MySoftware.aspx).
5. Une Office est installée, ***n’ouvrez*** ni ne connectez-vous à Office applications.
6. Sur le serveur RDS, activez l’activation d’ordinateurs partagés en éditant le Registre en suivant les étapes suivantes :
   1. Cliquez avec le bouton droit Windows dans le coin inférieur gauche de votre écran, puis sélectionnez **Exécuter.** Dans la zone Ouvrir, tapez **regedit** puis cliquez sur **OK**.
   2. Sélectionnez **Oui** lorsque vous y invitez l’Éditeur du Registre pour apporter des modifications à votre appareil.
   3. Dans l’Éditeur du Registre, ajoutez une valeur de chaîne **sharedComputerLicensing** avec le paramètre 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Sur le serveur RDS, ***connectez-vous*** en tant qu’utilisateur final et vérifiez que l’activation d’ordinateurs [partagés](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)est activée pour Applications Microsoft 365 pour les grandes entreprises .
