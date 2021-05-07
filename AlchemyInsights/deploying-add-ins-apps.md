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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233522"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="fa62b-102">Déploiement de Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="fa62b-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="fa62b-103">Le déploiement centralisé est le moyen recommandé pour déployer des Office aux utilisateurs et groupes au sein de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="fa62b-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="fa62b-104">Pour déployer des modules, suivez les étapes ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="fa62b-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="fa62b-105">**Remarque :** Pour installer des Office en tant qu’utilisateur individuel, voir Afficher, gérer et installer des Office [programmes.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="fa62b-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="fa62b-106">Assurez-vous également que l’acquisition individuelle de Office store est activée.</span><span class="sxs-lookup"><span data-stu-id="fa62b-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="fa62b-107">Pour plus d’informations, voir Empêcher les téléchargements de Office store sur tous les [clients (sauf Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="fa62b-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="fa62b-108">Assurez-vous que votre environnement répond aux exigences de déploiement de modules à l’aide d’un déploiement centralisé.</span><span class="sxs-lookup"><span data-stu-id="fa62b-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="fa62b-109">Pour plus d’informations, voir [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="fa62b-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="fa62b-110">Go to **Paramètres**  >  **Integrated Apps** Get  >  **apps** in the Microsoft 365 admin center to deploy add-ins.</span><span class="sxs-lookup"><span data-stu-id="fa62b-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="fa62b-111">Remarques :</span><span class="sxs-lookup"><span data-stu-id="fa62b-111">Notes:</span></span> 

- <span data-ttu-id="fa62b-112">Les applications intégrées nécessitent que l’administrateur dispose des autorisations d’administrateur Exchange administrateur global.</span><span class="sxs-lookup"><span data-stu-id="fa62b-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="fa62b-113">Lorsque vous déployez des modules pour plusieurs utilisateurs, nous vous recommandons d’effectuer des affectations à l’aide de groupes plutôt que d’utilisateurs individuels.</span><span class="sxs-lookup"><span data-stu-id="fa62b-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="fa62b-114">Pour plus d’informations, voir Considérations lors de l’affectation d’un [add-in à des utilisateurs et des groupes.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="fa62b-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="fa62b-115">Le déploiement centralisé ne prend pas en charge les utilisateurs des groupes imbrmbrés ou des groupes qui ont des groupes parents.</span><span class="sxs-lookup"><span data-stu-id="fa62b-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="fa62b-116">Pour plus d’informations, voir [Affectations d’utilisateurs et de groupes.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="fa62b-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="fa62b-117">Assurez-vous que le service de gestion des applications Microsoft 365 (GUID : '0517ffae-825d-4aff-999e-3f2336b8a20a') est activé pour que les utilisateurs se connectent.</span><span class="sxs-lookup"><span data-stu-id="fa62b-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="fa62b-118">Pour plus d’informations, voir [Configurer les propriétés de l’application.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="fa62b-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="fa62b-119">Si vous avez des problèmes lors du déploiement de vos applications intégrées, essayez de les déployer à l’aide [des applications intégrées.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="fa62b-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="fa62b-120">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="fa62b-120">For more information, see:</span></span>

<span data-ttu-id="fa62b-121">[Déployer des add-ins dans le Centre d’administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gérer les add-ins dans le Centre d’administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utiliser les cmdlets PowerShell de déploiement centralisé pour gérer les add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publier des Office à l’aide d’un déploiement centralisé via le Centre d Microsoft 365'administration](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Résolution des problèmes : l’utilisateur ne voit pas les modules](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Résoudre les erreurs de l’utilisateur Office des modules](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="fa62b-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>