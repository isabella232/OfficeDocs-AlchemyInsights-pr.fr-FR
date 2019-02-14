---
title: 1491-Search-not-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964857"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="99f45-102">Recherche de contenu ne retourne ne pas les résultats attendus</span><span class="sxs-lookup"><span data-stu-id="99f45-102">Content Search not returning expected results</span></span>

<span data-ttu-id="99f45-p101">Lors de l’exécution de recherches de contenu à partir du centre de conformité de & sécurité pour Microsoft Office 365, vous pouvez recevoir des résultats inattendus. Prenez en compte les éléments suivants peuvent avoir une incidence sur vos résultats de recherche :</span><span class="sxs-lookup"><span data-stu-id="99f45-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="99f45-p102">**Emplacements de contenu et des conditions de recherche**: Vérifiez que vous avez sélectionné les emplacements appropriés de contenu et les critères de recherche. Si vous avez exécuté une recherche de grande taille (avec nombreux emplacements), pensez à diviser en plusieurs recherches.</span><span class="sxs-lookup"><span data-stu-id="99f45-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="99f45-p103">**Partiellement des éléments indexés**: [partiellement des éléments indexés](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) de boîtes aux lettres sont inclus dans les résultats de recherche estimés. Toutefois, des éléments indexés partiellement à partir de sites dans SharePoint et OneDrive ne sont pas inclus dans l’estimation de la recherche.</span><span class="sxs-lookup"><span data-stu-id="99f45-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="99f45-p104">**Échecs de recherche**: lors de la recherche d’un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), vous obtiendrez des erreurs de recherche, avec des codes d’erreur tel que CS008-009 et CS012-002). Dans ce cas, réessayez la recherche uniquement pour les emplacements de contenu ayant échoués. Consultez [cet article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="99f45-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
