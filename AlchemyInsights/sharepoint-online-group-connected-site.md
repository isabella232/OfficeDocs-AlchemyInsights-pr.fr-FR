---
title: Ajouter un groupe à un site SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064391"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="7150f-102">Problèmes lors de la création d’un site connecté à un groupe dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="7150f-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="7150f-103">Certains problèmes courants lors de la création ou de la recréation d’un site connecté à un groupe.</span><span class="sxs-lookup"><span data-stu-id="7150f-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="7150f-104">Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.</span><span class="sxs-lookup"><span data-stu-id="7150f-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="7150f-105">Télécharger [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="7150f-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="7150f-106">Pour plus d’informations sur la prise en main de PowerShell, voir [Getting Started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="7150f-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="7150f-107">Supprimez le site des sites supprimés à l’aide de l’applet de commande PowerShell [Remove-spodeletedsit](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="7150f-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="7150f-108">PowerShell est nécessaire pour supprimer définitivement les sites de groupe.</span><span class="sxs-lookup"><span data-stu-id="7150f-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="7150f-109">Si vous créez un site connecté à un groupe et recevez un avertissement : **un autre groupe avec le même alias existe déjà**, vérifiez les groupes existants à partir du [Centre d’administration Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="7150f-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="7150f-110">Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez-en un autre.</span><span class="sxs-lookup"><span data-stu-id="7150f-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="7150f-111">Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7150f-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="7150f-112">Vous pouvez connecter des sites existants à un groupe Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7150f-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="7150f-113">Pour plus d’informations, consultez [la rubrique connecter un groupe Microsoft 365 à l’aide de l’interface utilisateur SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="7150f-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="7150f-114">Pour créer un site de groupe Microsoft 365 connecté, vous devez créer un [site d’équipe](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="7150f-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
