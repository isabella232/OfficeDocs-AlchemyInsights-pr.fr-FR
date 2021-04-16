---
title: Outil d’exportation de la découverte électronique
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814586"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="c6843-102">Vous ne pouvez pas installer ou exécuter l'outil d'exportation eDiscovery ?</span><span class="sxs-lookup"><span data-stu-id="c6843-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="c6843-103">Si vous ne pouvez pas installer ou exécuter l'outil d'exportation eDiscovery pour télécharger les résultats de recherche, vérifiez les points suivants :</span><span class="sxs-lookup"><span data-stu-id="c6843-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="c6843-104">L'ordinateur que vous utilisez répond aux conditions préalables ci-après :</span><span class="sxs-lookup"><span data-stu-id="c6843-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="c6843-105">versions 32 ou 64 bits de Windows 7 et versions ultérieures</span><span class="sxs-lookup"><span data-stu-id="c6843-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="c6843-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="c6843-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="c6843-107">un navigateur pris en charge :</span><span class="sxs-lookup"><span data-stu-id="c6843-107">A supported browser:</span></span>

  - <span data-ttu-id="c6843-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c6843-108">Microsoft Edge</span></span>

    <span data-ttu-id="c6843-109">Ou</span><span class="sxs-lookup"><span data-stu-id="c6843-109">Or</span></span>

  - <span data-ttu-id="c6843-110">Internet Explorer 10 et versions ultérieures</span><span class="sxs-lookup"><span data-stu-id="c6843-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="c6843-111">Les autres navigateurs, tels que Google Chrome et Mozilla Firefox, ne sont pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="c6843-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="c6843-112">Votre organisation peut se connecter au point de terminaison dans Azure, qui est **\* .blob.core.windows.net** (le caractère générique représente un identificateur unique pour votre travail d'exportation).</span><span class="sxs-lookup"><span data-stu-id="c6843-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="c6843-113">Le rôle Exporter vous est attribué dans le Centre de conformité de sécurité Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="c6843-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="c6843-114">Par défaut, ce rôle est attribué uniquement au groupe de rôles Gestionnaire eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="c6843-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="c6843-115">Voir [Attribuer des autorisations eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="c6843-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="c6843-116">Pour plus d'informations, [voir Exporter les résultats de la recherche de contenu.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="c6843-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="c6843-117">Si vous exportez plus de 100 000 boîtes aux lettres, vous devrez utiliser le Powershell suivant pour télécharger les résultats de l'exportation : Exportation des résultats de plus de  [100 000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c6843-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>