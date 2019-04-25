---
title: 1491-ne pas renvoyer-résultats attendus
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383833"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="394aa-102">Recherche de contenu ne renvoyant pas les résultats attendus</span><span class="sxs-lookup"><span data-stu-id="394aa-102">Content Search not returning expected results</span></span>

<span data-ttu-id="394aa-103">Lors de l'exécution de recherches de contenu à partir du centre de sécurité & Office 365 Security, il se peut que vous receviez des résultats inattendus.</span><span class="sxs-lookup"><span data-stu-id="394aa-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="394aa-104">Tenez compte des éléments suivants qui peuvent avoir une incidence sur vos résultats de recherche:</span><span class="sxs-lookup"><span data-stu-id="394aa-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="394aa-105">**Emplacements de contenu et conditions de recherche**: Assurez-vous que vous avez sélectionné les emplacements de contenu et les conditions de recherche appropriés.</span><span class="sxs-lookup"><span data-stu-id="394aa-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="394aa-106">Si vous avez exécuté une recherche volumineuse (avec de nombreux emplacements), envisagez de la fractionner en plusieurs recherches.</span><span class="sxs-lookup"><span data-stu-id="394aa-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="394aa-107">**Éléments partiellement indexés**: les [éléments partiellement indexés](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) des boîtes aux lettres sont inclus dans les résultats de recherche estimés.</span><span class="sxs-lookup"><span data-stu-id="394aa-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="394aa-108">Toutefois, les éléments partiellement indexés des sites dans SharePoint et OneDrive ne sont pas inclus dans l'estimation de la recherche.</span><span class="sxs-lookup"><span data-stu-id="394aa-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="394aa-109">**Échecs de recherche**: lors de la recherche dans un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), vous pouvez obtenir des erreurs de recherche, avec des codes d'erreur comme CS008-009 et CS012-002).</span><span class="sxs-lookup"><span data-stu-id="394aa-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="394aa-110">Dans ce cas, effectuez une nouvelle tentative de recherche uniquement pour les emplacements de contenu ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="394aa-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="394aa-111">Pour plus d'informations, consultez [cet article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="394aa-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
