---
title: Créer un site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806937"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="0cb4d-102">Créer un site SharePoint</span><span class="sxs-lookup"><span data-stu-id="0cb4d-102">Create a SharePoint site</span></span>

<span data-ttu-id="0cb4d-103">Créer ou gérer des sites à partir de [sites actifs](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) dans le centre d’administration SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="0cb4d-104">Pour plus d’informations, consultez [la rubrique gérer les sites dans le nouveau centre d’administration SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="0cb4d-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="0cb4d-105">Bourgeon</span><span class="sxs-lookup"><span data-stu-id="0cb4d-105">Tips:</span></span>

- <span data-ttu-id="0cb4d-106">Vous **ne pouvez pas** créer un site avec la même URL d’un site existant.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="0cb4d-107">Si vous avez supprimé un site et souhaitez réutiliser l’URL, il est possible que le site supprimé existe toujours sous [sites supprimés](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="0cb4d-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="0cb4d-108">Le site devra être supprimé définitivement pour réutiliser l’URL.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="0cb4d-109">Pour supprimer complètement un site avec PowerShell, consultez l’exemple d’applet de commande [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="0cb4d-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="0cb4d-110">Certains utilisateurs peuvent ne pas être en mesure de créer un site.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="0cb4d-111">[Consultez la rubrique Manage site Creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="0cb4d-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="0cb4d-112">Il est possible que le site semble bloqué lorsque la **création** est plus longue que prévu.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="0cb4d-113">Si plus de 24 heures se sont écoulées depuis le début de ce problème, veuillez consigner un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="0cb4d-114">Dans de nombreux cas, nous travaillons déjà sur une solution.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0cb4d-115">Veuillez nous fournir au moins 24 heures pour terminer une solution.</span><span class="sxs-lookup"><span data-stu-id="0cb4d-115">Please give us at least 24 hours to complete a solution.</span></span>
