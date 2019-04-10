---
title: Le partage avec des utilisateurs externes ne fonctionne pas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747596"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="cb7c5-102">Résoudre les problèmes de partage de contenu SharePoint avec des utilisateurs externes</span><span class="sxs-lookup"><span data-stu-id="cb7c5-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="cb7c5-103">Assurez-vous que le partage externe est activé pour votre organisation:</span><span class="sxs-lookup"><span data-stu-id="cb7c5-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="cb7c5-104">Accédez à la [page &amp; compléments de services dans le centre d'administration 365 de Microsoft](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), puis cliquez sur **sites**.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="cb7c5-105">Assurez-vous que le paramètre est activé.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="cb7c5-106">Si «uniquement les utilisateurs externes existants» est sélectionné, assurez-vous que l'utilisateur externe est affiché dans le centre d'administration 365 de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="cb7c5-107">Assurez-vous que le partage externe est activé pour le site.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="cb7c5-108">Pour une collection de sites classique:</span><span class="sxs-lookup"><span data-stu-id="cb7c5-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="cb7c5-109">Dans le nouveau centre d'administration SharePoint, dans le volet de gauche, cliquez sur **sites**.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="cb7c5-110">Sélectionnez le ou les sites et, dans le ruban, cliquez sur **partage**.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="cb7c5-111">Pour un site d'équipe appartenant à un groupe Office 365 ou à un site de communication:</span><span class="sxs-lookup"><span data-stu-id="cb7c5-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="cb7c5-112">Ces nouveaux types de sites ont le même paramètre de partage que votre paramètre à l'échelle de votre organisation, sauf si le paramètre à l'échelle de l'organisation autorise le partage de fichiers à l'aide de liens ne nécessitant pas de connexion.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="cb7c5-113">Dans ce cas, les sites autorisent le partage avec des utilisateurs externes nouveaux et existants qui se connectent.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="cb7c5-114">Pour modifier le paramètre de sites spécifiques, utilisez le nouveau centre d'administration SharePoint ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="cb7c5-115">[En savoir plus](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="cb7c5-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="cb7c5-116">Le paramètre de partage externe de n'importe quel site peut être plus restrictif que le paramètre à l'échelle de votre organisation, mais pas plus permissif que le paramètre à l'échelle de l'organisation.</span><span class="sxs-lookup"><span data-stu-id="cb7c5-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

