---
title: Restaurer un site supprimé
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048794"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="52540-102">Restaurer un site supprimé</span><span class="sxs-lookup"><span data-stu-id="52540-102">Restore a deleted site</span></span>

<span data-ttu-id="52540-103">Lorsqu’un administrateur supprime un site SharePoint, il est placé dans la corbeille de la collection de sites, où il est conservé pendant 93 jours avant d’être définitivement supprimé.</span><span class="sxs-lookup"><span data-stu-id="52540-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="52540-104">Pour restaurer le site :</span><span class="sxs-lookup"><span data-stu-id="52540-104">To restore the site:</span></span>
  
1. <span data-ttu-id="52540-105">Dans le nouveau centre d’administration SharePoint, cliquez sur **Corbeille** sur le ruban.</span><span class="sxs-lookup"><span data-stu-id="52540-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="52540-106">Activez la case à cocher en regard de la collection de sites à restaurer.</span><span class="sxs-lookup"><span data-stu-id="52540-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="52540-107">Cliquez sur **restaurer les éléments supprimés**.</span><span class="sxs-lookup"><span data-stu-id="52540-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="52540-108">Pour restaurer un site de communication supprimé, vous pouvez utiliser le nouveau centre d’administration SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52540-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="52540-109">Dans le cas contraire, vous devez utiliser Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="52540-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="52540-110">Pour restaurer un site qui appartient à un groupe Office 365, vous devez restaurer le groupe dans le centre d’administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="52540-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="52540-111">Les groupes peuvent être restaurés pendant 30 jours après leur suppression.</span><span class="sxs-lookup"><span data-stu-id="52540-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

