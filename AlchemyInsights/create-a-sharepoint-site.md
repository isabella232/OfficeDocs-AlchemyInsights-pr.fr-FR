---
title: Créer un site SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515805"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7f0e5-102">Créer un site SharePoint</span><span class="sxs-lookup"><span data-stu-id="7f0e5-102">Create a SharePoint site</span></span>

<span data-ttu-id="7f0e5-103">Pour plus d’informations sur la création de sites SharePoint, consultez les rubriques suivantes:</span><span class="sxs-lookup"><span data-stu-id="7f0e5-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="7f0e5-104">[Gérer les sites dans le nouveau centre d’administration SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Découvrez les options de création de sites, notamment la création d’un site classique ou d’un site teams qui n’inclut pas de groupe Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="7f0e5-105">[Créer un site d’équipe dans SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Découvrez comment créer un site d’équipe.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="7f0e5-106">[Créer un site de communication dans SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Découvrez comment créer un site de communication.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="7f0e5-107">[Gérer les sites dans le nouveau centre d’administration SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Découvrez comment créer un site classique ou un site d’équipe qui n’inclut pas un groupe Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="7f0e5-108">[! Bourgeon</span><span class="sxs-lookup"><span data-stu-id="7f0e5-108">[!Tips]</span></span>
> - <span data-ttu-id="7f0e5-109">Vous ne pouvez pas créer un site avec la même URL d’un site existant.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7f0e5-110">Si vous avez supprimé un site et souhaitez réutiliser l’URL, il est possible que le site supprimé existe toujours sous **sites supprimés**.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="7f0e5-111">Pour gérer les sites supprimés, consultez [la rubrique supprimer un site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="7f0e5-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="7f0e5-112">Pour supprimer complètement un site avec PowerShell, consultez l’exemple d’applet de commande [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="7f0e5-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="7f0e5-113">Certains utilisateurs peuvent ne pas être en mesure de créer un site.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="7f0e5-114">Consultez la rubrique [Manage site Creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7f0e5-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="7f0e5-115">Il est possible que le site semble bloqué lorsque la **création** est plus longue que prévu.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7f0e5-116">Si plus de 24 heures se sont écoulées depuis le début de ce problème, veuillez consigner un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7f0e5-117">Dans de nombreux cas, nous travaillons déjà sur une solution.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7f0e5-118">Veuillez nous fournir au moins 24 heures pour terminer une solution.</span><span class="sxs-lookup"><span data-stu-id="7f0e5-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="7f0e5-119">Si vous devez créer un site d’équipe qui n’inclut pas de groupe Office 365,</span><span class="sxs-lookup"><span data-stu-id="7f0e5-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


