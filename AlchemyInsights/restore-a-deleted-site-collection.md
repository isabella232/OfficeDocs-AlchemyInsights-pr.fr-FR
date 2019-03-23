---
title: Restaurer une collection de sites supprimée
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753784"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="01c31-102">Restaurer une collection de sites supprimée</span><span class="sxs-lookup"><span data-stu-id="01c31-102">Restore a deleted site collection</span></span>

<span data-ttu-id="01c31-103">Lorsqu'un administrateur supprime une collection de sites classique, elle est placée dans la corbeille de la collection de sites, où elle est conservée pendant 93 jours avant d'être définitivement supprimée.</span><span class="sxs-lookup"><span data-stu-id="01c31-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="01c31-104">Pour restaurer la collection de sites:</span><span class="sxs-lookup"><span data-stu-id="01c31-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="01c31-105">Dans le centre d'administration SharePoint classique, cliquez sur **Corbeille** dans le ruban.</span><span class="sxs-lookup"><span data-stu-id="01c31-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="01c31-106">Activez la case à cocher en regard de la collection de sites à restaurer.</span><span class="sxs-lookup"><span data-stu-id="01c31-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="01c31-107">Cliquez sur **restaurer les éléments supprimés**.</span><span class="sxs-lookup"><span data-stu-id="01c31-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="01c31-108">Pour restaurer un site de communication supprimé, vous pouvez utiliser le nouvel aperçu du centre d'administration SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01c31-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="01c31-109">Dans le cas contraire, vous devez utiliser PowerShell.</span><span class="sxs-lookup"><span data-stu-id="01c31-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="01c31-110">Pour restaurer un site qui appartient à un groupe Office 365, vous devez restaurer le groupe dans le centre d'administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="01c31-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="01c31-111">Les groupes peuvent être restaurés pendant 30 jours après leur suppression.</span><span class="sxs-lookup"><span data-stu-id="01c31-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

