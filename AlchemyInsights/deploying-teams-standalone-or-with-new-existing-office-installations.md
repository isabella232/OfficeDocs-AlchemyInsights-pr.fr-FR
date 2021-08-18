---
title: Déploiement de Teams autonomes ou avec des installations de Office nouvelles ou existantes
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320120"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Déploiement de Teams autonomes ou avec des installations de Office nouvelles ou existantes

Microsoft Teams est désormais inclus dans le cadre des nouvelles ***installations*** de Applications Microsoft 365 pour les grandes entreprises, Applications Microsoft 365 pour les PME et Office pour Mac. Pour plus d’informations, [voir Quand les Microsoft Teams seront-elles](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps) incluses dans les nouvelles installations de Office ?

En outre, à partir de la version 1906 du canal actuel, Teams est ajouté aux ***installations*** existantes de Applications Microsoft 365 pour les grandes entreprises (et Applications Microsoft 365 pour les PME) sur les appareils exécutant Windows lorsque vous mettez à jour votre installation existante vers la dernière version. Pour plus d’informations, [voir Qu’en est-il des installations](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps) existantes de Office ?

**Remarque**: si vous ne souhaitez pas attendre cette planification de déploiement, vous pouvez déployer Teams en tant que serveur autonome pour vos utilisateurs en suivant ces [instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ou vous pouvez faire installer des Teams pour eux-mêmes à partir de [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Si votre organisation n’est pas prête à déployer des Teams, nous avons les [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) étapes à suivre pour exclure les ***Teams*** des [installations](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) nouvelles ou existantes de Office. Si vous souhaitez que Teams soit installé, mais que vous ne souhaitez pas que Teams démarre automatiquement pour l’utilisateur après son installation, voir Empêcher Microsoft Teams de démarrer automatiquement après [l’installation.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Pour ***désinstaller Teams*** à partir d’un appareil exécutant Windows, voir [Désinstaller Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pour nettoyer les Microsoft Teams à partir de plusieurs ordinateurs ou utilisateurs cibles, voir [Microsoft Teams le nettoyage du déploiement.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Si vous utilisez des [ordinateurs partagés,](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)des services Bureau à distance (RDS) ou une infrastructure VDI (Virtual Desktop Infrastructure), voir Ordinateur partagé et environnements VDI avec Microsoft Teams .

Si vous utilisez Office pour Mac, voir Microsoft Teams [installations sur un Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Remarque**: une Teams est installée, [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) elle est automatiquement mise à jour environ toutes les deux semaines avec de nouvelles fonctionnalités et des mises à jour qualité. 