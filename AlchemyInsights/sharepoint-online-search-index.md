---
title: Recherche dans SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044041"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="60c77-102">Analyse et indexation de contenu dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="60c77-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="60c77-103">Le contenu doit être analysé et ajouté à l’index de recherche pour que les utilisateurs puissent trouver ce qu’ils recherchent dans SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="60c77-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="60c77-104">Le contenu est automatiquement analysé en fonction d’une planification d’analyse prédéfinie (la planification d’analyse ne peut pas être modifiée).</span><span class="sxs-lookup"><span data-stu-id="60c77-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="60c77-105">Le robot récupère le contenu qui a été modifié depuis la dernière analyse et met à jour l’index.</span><span class="sxs-lookup"><span data-stu-id="60c77-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="60c77-106">Pour vous assurer que le contenu est analysé et que l’index est mis à jour, notez les points suivants :</span><span class="sxs-lookup"><span data-stu-id="60c77-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="60c77-107">Assurez-vous que le contenu peut être trouvé en [effectuant une recherche](https://docs.microsoft.com/sharepoint/make-site-content-searchable)dans le contenu de site.</span><span class="sxs-lookup"><span data-stu-id="60c77-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="60c77-108">Lorsque vous avez modifié une propriété gérée, ou lorsque vous avez modifié le mappage des propriétés analysées et gérées, le site doit être ré-analysé pour que vos modifications soient reflétées dans l’index de recherche.</span><span class="sxs-lookup"><span data-stu-id="60c77-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="60c77-109">Étant donné que vos modifications sont apportées dans le schéma de recherche, et non au site réel, le robot ne réindexe pas automatiquement le site.</span><span class="sxs-lookup"><span data-stu-id="60c77-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="60c77-110">Pour plus d’informations, voir [demander manuellement l’analyse et la réindexation d’un site, d’une bibliothèque ou d’une liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="60c77-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="60c77-111">Patientez au moins 24 heures après avoir demandé manuellement une analyse et une réindexation complète pour voir si vous rencontrez toujours un problème.</span><span class="sxs-lookup"><span data-stu-id="60c77-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="60c77-112">Si plus de 24 heures se sont écoulées depuis l’ouverture de l’analyse et de la réindexation complète, veuillez consigner un cas de support.</span><span class="sxs-lookup"><span data-stu-id="60c77-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="60c77-113">Dans de nombreux cas, nous travaillons déjà sur une solution.</span><span class="sxs-lookup"><span data-stu-id="60c77-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="60c77-114">Veuillez nous fournir au moins 24 heures pour terminer une solution.</span><span class="sxs-lookup"><span data-stu-id="60c77-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="60c77-115">Si un site, un document (bibliothèque) ou une liste a été supprimé et s’affiche toujours dans les résultats de la recherche, les utilisateurs doivent recevoir une **erreur 404 Fichier introuvable** lors de la tentative d’accès.</span><span class="sxs-lookup"><span data-stu-id="60c77-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="60c77-116">Ce problème doit être consigné dans le cadre d’une demande d’assistance supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="60c77-116">This issue should be logged as a support case for further investigation.</span></span> 



