---
title: Déploiement de teams en tant que autonome ou avec des installations Office nouvelles ou existantes
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704631"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Déploiement de teams en tant que autonome ou avec des installations Office nouvelles ou existantes

Microsoft teams est désormais inclus dans le cadre des ***nouvelles installations*** d’applications Microsoft 365 pour les entreprises, de Microsoft 365 applications pour les entreprises et d’Office pour Mac. Pour plus d’informations, consultez la rubrique [quand Microsoft teams commencera-t-il à être inclus avec les nouvelles installations d’Office ?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

En outre, à partir de la version 1906 du canal mensuel, teams est ***ajouté aux installations existantes*** d’applications Microsoft 365 pour Enterprise (et Microsoft 365 apps pour les entreprises) sur les appareils exécutant Windows lorsque vous mettez à jour votre installation existante vers la dernière version. Pour plus d’informations, consultez [qu’en est-il des installations d’Office existantes ?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Si vous ne souhaitez pas attendre cette planification de déploiement, vous pouvez déployer teams en tant que autonome pour vos utilisateurs en [suivant ces instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ou vous pouvez faire en sorte que vos [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)utilisateurs installent teams pour eux-mêmes.

Si votre organisation n’est pas prête à déployer Teams, nous vous recommandons de suivre les étapes à suivre pour ***exclure teams*** des installations [nouvelles](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) ou [existantes](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) d’Office. Si vous souhaitez que teams soit installé, mais que vous ne voulez pas que teams démarre automatiquement pour l’utilisateur après son installation, consultez la rubrique [empêcher Microsoft teams de démarrer automatiquement après l’installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Pour ***désinstaller teams*** d’un appareil exécutant Windows, reportez-vous à la rubrique [Uninstall Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pour nettoyer Microsoft teams de plusieurs ordinateurs cibles ou utilisateurs, consultez la rubrique [nettoyage du déploiement de Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Si vous utilisez des ordinateurs partagés, des services Bureau à distance (RDS) ou une infrastructure VDI (Virtual Desktop Infrastructure), consultez la rubrique [environnements d’ordinateurs et VDI partagés avec Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Si vous utilisez Office pour Mac, consultez [la rubrique installations de Microsoft teams sur un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Une fois teams installé, il est [automatiquement mis à jour](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) environ toutes les deux semaines avec les nouvelles fonctionnalités et les mises à jour de qualité. 