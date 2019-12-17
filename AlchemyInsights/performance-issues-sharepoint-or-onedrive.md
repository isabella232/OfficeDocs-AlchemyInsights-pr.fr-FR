---
title: Problèmes de performances-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068398"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="8c519-102">SharePoint ou OneDrive est lent, inaccessible ou indisponible pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8c519-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="8c519-103">SharePoint ou OneDrive sont peut-être lents, inaccessibles ou indisponibles, ou peuvent afficher le service non disponible ou des erreurs 503, pour plusieurs raisons :</span><span class="sxs-lookup"><span data-stu-id="8c519-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="8c519-104">Si votre site SharePoint ou OneDrive est lent ou retardé pour plusieurs utilisateurs, il peut y avoir un problème de service temporaire dans lequel les utilisateurs subissent des retards ou des erreurs de navigation intermittents lors de l’accès à des sites SharePoint ou à du contenu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8c519-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="8c519-105">Consultez le [tableau de bord d’État du service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour voir si votre organisation est concernée.</span><span class="sxs-lookup"><span data-stu-id="8c519-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="8c519-106">Les utilisateurs peuvent recevoir un message d’erreur « le *serveur 503 est occupé* » lors de la tentative de navigation vers des sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8c519-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="8c519-107">Cette erreur peut être causée par la limitation dans le service SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8c519-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="8c519-108">SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8c519-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="8c519-109">Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources.</span><span class="sxs-lookup"><span data-stu-id="8c519-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="8c519-110">Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="8c519-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="8c519-111">Si vous constatez un ralentissement des performances avec un site ou une page SharePoint **classique** ou **moderne** , utilisez l' [outil de diagnostic de page](https://aka.ms/perftool) pour analyser les pages.</span><span class="sxs-lookup"><span data-stu-id="8c519-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="8c519-112">Si les performances générales sont toujours déchargées, consultez les ressources au bas de cet article : [Présentation de l’optimisation des performances pour SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="8c519-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  