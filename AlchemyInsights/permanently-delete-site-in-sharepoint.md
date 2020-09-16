---
title: Supprimer définitivement un site dans SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771719"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="2506b-102">Supprimer définitivement un site dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="2506b-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="2506b-103">Pour réutiliser une URL à partir d’un site supprimé (pour recréer un site) ou pour supprimer définitivement un site, car il n’est plus utilisé, vous pouvez utiliser **Supprimer définitivement** du nouveau centre d’administration SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2506b-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="2506b-104">Accédez à la [Page de sites supprimées du nouveau Centre d’administration SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) et connectez-vous à l’aide d’un compte disposant des autorisations d’administrateur pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="2506b-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="2506b-105">Dans la colonne de gauche, sélectionnez un site.</span><span class="sxs-lookup"><span data-stu-id="2506b-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="2506b-106">Cliquez sur **supprimer définitivement**.</span><span class="sxs-lookup"><span data-stu-id="2506b-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="2506b-107">**Remarque**: les sites connectés au groupe ne peuvent pas être supprimés définitivement du nouveau centre d’administration SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2506b-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="2506b-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) devra être utilisé à la place.</span><span class="sxs-lookup"><span data-stu-id="2506b-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="2506b-109">Pour plus d'informations, consultez la rubrique [Suppression définitive d’un site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="2506b-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
