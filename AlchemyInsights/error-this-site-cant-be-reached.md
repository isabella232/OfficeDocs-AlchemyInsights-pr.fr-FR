---
title: 'Ce site n’est pas accessible : erreur lors de la tentative d’accès au site SharePoint à partir du navigateur ou de Teams'
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718183"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="bb59a-102">Erreur « Ce site n’est pas accessible » lors de la tentative d’accès au site SharePoint à partir du navigateur ou de Teams</span><span class="sxs-lookup"><span data-stu-id="bb59a-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="bb59a-103">Les utilisateurs peuvent recevoir l’erreur « Ce site n’est pas accessible » lorsque vous essayez d’accéder au site SharePoint à partir du navigateur ou de Teams.</span><span class="sxs-lookup"><span data-stu-id="bb59a-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="bb59a-104">Pour résoudre ce problème :</span><span class="sxs-lookup"><span data-stu-id="bb59a-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="bb59a-105">Vérifiez si la page d’accueil se trouve dans la Corbeille ou la Corbeille second niveau et restituer la page.</span><span class="sxs-lookup"><span data-stu-id="bb59a-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="bb59a-106">**Exemple d’URL directe vers la Corbeille**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="bb59a-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="bb59a-107">Si la page d’accueil est définitivement supprimée de la Corbeille, créez une page de site à partir de la bibliothèque pages du site et faites-en une page d’accueil.</span><span class="sxs-lookup"><span data-stu-id="bb59a-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="bb59a-108">**Exemple d’URL directe**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="bb59a-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>