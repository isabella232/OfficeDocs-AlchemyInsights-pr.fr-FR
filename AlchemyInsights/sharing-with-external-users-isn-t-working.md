---
title: Partage avec des utilisateurs externes ne fonctionne pas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900866"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="2e853-102">Résoudre les problèmes de partage de contenu SharePoint avec des utilisateurs externes</span><span class="sxs-lookup"><span data-stu-id="2e853-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="2e853-103">Assurez-vous que le partage externe est activé pour votre organisation :</span><span class="sxs-lookup"><span data-stu-id="2e853-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="2e853-104">Accédez à la [Services &amp; page des compléments dans le centre d’administration Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), cliquez sur **Sites**.</span><span class="sxs-lookup"><span data-stu-id="2e853-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="2e853-p101">Assurez-vous que le paramètre est activé sur « On ». Si « Utilisateurs externes existants uniquement » sont sélectionnées, assurez-vous que l’utilisateur externe est répertorié dans le centre d’administration d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e853-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="2e853-p102">Assurez-vous qu’externe partage activé pour le site. Pour une collection de sites classique :</span><span class="sxs-lookup"><span data-stu-id="2e853-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="2e853-109">Dans le centre d’administration SharePoint classique, dans le volet gauche, cliquez sur **des collections de sites**.</span><span class="sxs-lookup"><span data-stu-id="2e853-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="2e853-110">Sélectionnez l’ou les sites, dans le ruban, cliquez sur **partage**.</span><span class="sxs-lookup"><span data-stu-id="2e853-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="2e853-111">Pour un site d’équipe qui appartient à un groupe d’Office 365, ou un site de communication :</span><span class="sxs-lookup"><span data-stu-id="2e853-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="2e853-p103">Ces nouveaux types de sites ont le même paramètre partage en tant que paramètre de l’échelle de l’organisation, à moins que le paramètre d’échelle de l’organisation permet le partage de fichiers à l’aide de liens qui ne nécessitent pas de connexion. Dans ce cas, les sites autoriser le partage avec des utilisateurs externes qui se connectent à. Pour modifier le paramètre pour des sites spécifiques, utilisez le nouveau centre d’administration SharePoint (preview) ou PowerShell. [En savoir plus](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="2e853-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="2e853-116">Le paramètre partage externe pour un site peut être plus restrictif que votre paramètre de l’organisation, mais pas plus permissif que le paramètre de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="2e853-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

