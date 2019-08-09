---
title: Gérer le schéma de recherche dans SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270100"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="6a58f-102">Gérer le schéma de recherche dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6a58f-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="6a58f-103">Le schéma de recherche contrôle les éléments que les utilisateurs peuvent rechercher, la façon dont les utilisateurs peuvent y effectuer des recherches, ainsi que la façon dont vous pouvez présenter les résultats sur vos sites Web de recherche.</span><span class="sxs-lookup"><span data-stu-id="6a58f-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="6a58f-104">Pour savoir comment procéder [, voir gérer le schéma de recherche dans SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) :</span><span class="sxs-lookup"><span data-stu-id="6a58f-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="6a58f-105">Modifier le schéma de recherche.</span><span class="sxs-lookup"><span data-stu-id="6a58f-105">Change the search schema.</span></span>
- <span data-ttu-id="6a58f-106">Créer des propriétés gérées.</span><span class="sxs-lookup"><span data-stu-id="6a58f-106">Create managed properties.</span></span>
- <span data-ttu-id="6a58f-107">Mapper des propriétés analysées de mappage analysées sur des propriétés gérées.</span><span class="sxs-lookup"><span data-stu-id="6a58f-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="6a58f-108">Notez les points suivants en matière de gestion de votre schéma de recherche:</span><span class="sxs-lookup"><span data-stu-id="6a58f-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="6a58f-109">Si vous recevez un avertissement indiquant que **l’application est suspendue** lors d’une modification de schéma, il s’agit uniquement d’une situation temporaire car une maintenance de service est en cours.</span><span class="sxs-lookup"><span data-stu-id="6a58f-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="6a58f-110">Si plus de 24 heures se sont écoulées et que vous rencontrez toujours l’avertissement, veuillez consigner un cas de support.</span><span class="sxs-lookup"><span data-stu-id="6a58f-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="6a58f-111">Lorsque vous modifiez des propriétés gérées ou en ajoutez de nouvelles, les modifications ne prennent effet qu’une fois que le contenu a été ré-analysé.</span><span class="sxs-lookup"><span data-stu-id="6a58f-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="6a58f-112">Dans SharePoint Online, l’analyse s’effectue automatiquement en fonction de la planification d’analyse définie.</span><span class="sxs-lookup"><span data-stu-id="6a58f-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="6a58f-113">Pour vous assurer que vos modifications sont analysées, vous pouvez [demander spécifiquement une réindexation de la liste ou de la bibliothèque](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="6a58f-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="6a58f-114">Pour obtenir une vue d’ensemble du schéma de recherche, consultez la rubrique [Présentation du schéma de recherche](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="6a58f-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


