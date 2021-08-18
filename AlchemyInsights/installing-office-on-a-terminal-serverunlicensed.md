---
title: Installation d’office sur un serveur Terminal Server - Sans permis
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321997"
---
# <a name="installing-office-on-a-terminal-server"></a>Installation de Office sur un serveur Terminal Server

Pour le déploiement Applications Microsoft 365 pour les grandes entreprises sur un serveur Windows à l’aide des services Bureau à distance (RDS), anciennement nommés Services Terminal Server :
  
- Vous devez avoir un abonnement Microsoft 365 qui inclut des Applications Microsoft 365 pour les grandes entreprises, tels que Office 365 Entreprise E3 ou Enterprise E5. Les plans Applications Microsoft 365 pour les PME et Applications Microsoft 365 pour les PME Premium ne comprennent pas de Applications Microsoft 365 pour les grandes entreprises.

- Vous devez activer [l’activation d’ordinateurs partagés.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Si vous souhaitez installer Applications Microsoft 365 pour les grandes entreprises sur RDS à partir du Centre d’administration Microsoft 365, qui utilise les ***paramètres d’installation*** par défaut, utilisez les étapes suivantes.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Vérifiez le Microsoft 365 abonnement que vous avez. [En savoir plus](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Si nécessaire, passez à un autre abonnement Microsoft 365 abonnement. [En savoir plus](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Si Office est déjà installé sur le serveur RDS à l’aide d’Microsoft 365 abonnements, désinstallez-le. Par exemple, en allant dans le Panneau de commande \> Désinstaller un programme. Désinstallez [l’Assistant Support et récupération](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft si vous avez des problèmes.

4. Sur le serveur RDS, connectez-vous au Centre d’administration Microsoft 365 avec votre compte d’administrateur et [installez Applications Microsoft 365 pour les grandes entreprises](https://portal.office.com/OLS/MySoftware.aspx).

5. Une Office est installée, ***n’ouvrez*** ni ne connectez-vous à Office applications.

6. Sur le serveur RDS, activez l’activation d’ordinateurs partagés en éditant le Registre en suivant les étapes suivantes :

1. Cliquez avec le bouton droit Windows dans le coin inférieur gauche de votre écran, puis sélectionnez Exécuter. Dans la zone Ouvrir, tapez **regedit,** puis sélectionnez OK.

2. Sélectionnez Oui lorsque vous y invitez l’Éditeur du Registre pour apporter des modifications à votre appareil.

3. Dans l’Éditeur du Registre, ajoutez une valeur de chaîne **sharedComputerLicensing** avec le paramètre 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Sur le serveur RDS, ***connectez-vous*** en tant qu’utilisateur final et vérifiez que l’activation d’ordinateurs [partagés](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)est activée pour Applications Microsoft 365 pour les grandes entreprises .

Pour plus d’informations sur les conditions préalables, les instructions de configuration et les instructions sur les installations personnalisées à l’aide de l’outil déploiement Office, voir [Déployer Applications Microsoft 365 pour les grandes entreprises](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)à l’aide des services Bureau à distance.
  
Pour corriger les erreurs liées à l’activation d’ordinateurs [partagés,](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)consultez Résoudre les problèmes liés à l’activation d’ordinateurs partagés pour Applications Microsoft 365 pour les grandes entreprises .
  