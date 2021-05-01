---
title: Déploiement de Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107510"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Déploiement de Microsoft 365 Apps

Le déploiement centralisé est le moyen recommandé pour déployer des Office aux utilisateurs et groupes au sein de votre organisation. Pour déployer des modules, suivez les étapes ci-dessous :

**Remarque :** Pour installer des Office en tant qu'utilisateur individuel, voir Afficher, gérer et installer des Office [programmes.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Assurez-vous également que l'acquisition individuelle de Office store est activée. 

1. Assurez-vous que votre environnement répond aux exigences de déploiement de modules à l'aide d'un déploiement centralisé. Pour plus d'informations, voir [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Go to **Paramètres**  >  **Integrated Apps** Get  >  **apps** in the Microsoft 365 admin center to deploy add-ins. 

Remarques : 

- Les applications intégrées nécessitent que l'administrateur dispose des autorisations d'administrateur Exchange administrateur global.

- Lorsque vous déployez des modules pour plusieurs utilisateurs, nous vous recommandons d'effectuer des affectations à l'aide de groupes plutôt que d'utilisateurs individuels. Pour plus d'informations, voir Considérations lors de l'affectation d'un [add-in à des utilisateurs et des groupes.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Le déploiement centralisé ne prend pas en charge les utilisateurs des groupes imbrmbrés ou des groupes qui ont des groupes parents. Pour plus d'informations, voir [Affectations d'utilisateurs et de groupes.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Assurez-vous que le service de gestion des applications Microsoft 365 (GUID : '0517ffae-825d-4aff-999e-3f2336b8a20a') est activé pour que les utilisateurs se connectent. Pour plus d'informations, voir [Configurer les propriétés de l'application.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Si vous avez des problèmes lors du déploiement de vos applications intégrées, essayez de les déployer à l'aide [des applications intégrées.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Pour plus d’informations, reportez-vous aux rubriques suivantes :

[Déployer des add-ins dans le Centre d'administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gérer les add-ins dans le Centre d'administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utiliser les cmdlets PowerShell de déploiement centralisé pour gérer les add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publier des Office à l'aide d'un déploiement centralisé via le Centre d Microsoft 365'administration](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Résolution des problèmes : l'utilisateur ne voit pas les modules](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Résoudre les erreurs de l'utilisateur Office des modules](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)