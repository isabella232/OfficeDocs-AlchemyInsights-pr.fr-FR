---
title: Le contenu n’apparaît pas dans les résultats de la recherche SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517029"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="8653e-102">Le contenu n’apparaît pas dans les résultats de la recherche SharePoint</span><span class="sxs-lookup"><span data-stu-id="8653e-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="8653e-103">Suivez ces étapes de résolution des problèmes lorsque le contenu attendu n’apparaît pas dans les résultats de la recherche:</span><span class="sxs-lookup"><span data-stu-id="8653e-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="8653e-104">Vérifiez que le **site** qui contient le contenu attendu est défini pour autoriser le contenu à apparaître dans les résultats de la recherche.</span><span class="sxs-lookup"><span data-stu-id="8653e-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="8653e-105">Suivez les étapes décrites dans [afficher le contenu d’un site dans les résultats de la recherche](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="8653e-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="8653e-106">Vérifiez que la **liste** ou la **bibliothèque** qui contient le contenu attendu est définie pour autoriser le contenu à apparaître dans les résultats de la recherche.</span><span class="sxs-lookup"><span data-stu-id="8653e-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="8653e-107">Suivez les étapes de la procédure [afficher le contenu de listes ou de bibliothèques dans les résultats](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)de la recherche.</span><span class="sxs-lookup"><span data-stu-id="8653e-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="8653e-108">Vérifiez que la page, le document ou la mise en page personnalisée est publié en tant que **version majeure.**</span><span class="sxs-lookup"><span data-stu-id="8653e-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="8653e-109">Suivez l’étape 3 dans la [recherche ne renvoie pas tous les résultats dans SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="8653e-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="8653e-110">Vérifiez que l’utilisateur dispose des **autorisations nécessaires** pour afficher le contenu.</span><span class="sxs-lookup"><span data-stu-id="8653e-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="8653e-111">Suivez les étapes de [Présentation des niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="8653e-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="8653e-112">Si le schéma de recherche a été modifié par l’ajout d’une nouvelle propriété gérée, par la modification d’une propriété gérée ou par la suppression d’une propriété gérée, une demande d’analyse et de réindexement sera requise.</span><span class="sxs-lookup"><span data-stu-id="8653e-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="8653e-113">\*\*\*\* Réindexer le contenu en suivant les étapes de la procédure de [demande d’analyse et de réindexation manuelle d’un site, d’une bibliothèque ou d’une liste](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="8653e-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="8653e-114">Cette opération peut prendre un certain temps, attendre 24 heures avant de vérifier à nouveau les résultats.</span><span class="sxs-lookup"><span data-stu-id="8653e-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="8653e-115">Pour plus d’informations, consultez [la rubrique activer le contenu d’un site pour pouvoir faire l’objet d’une recherche](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="8653e-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
