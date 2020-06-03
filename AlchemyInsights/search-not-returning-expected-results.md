---
title: 1491-ne pas renvoyer-résultats attendus
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510570"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="2f0d6-102">Recherche de contenu ne renvoyant pas les résultats attendus</span><span class="sxs-lookup"><span data-stu-id="2f0d6-102">Content Search not returning expected results</span></span>

<span data-ttu-id="2f0d6-103">Lors de l’exécution de recherches de contenu à partir du centre de conformité & Microsoft 365 Security, vous pouvez recevoir des résultats de recherche inattendus.</span><span class="sxs-lookup"><span data-stu-id="2f0d6-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="2f0d6-104">Tenez compte des éléments suivants qui peuvent avoir une incidence sur vos résultats de recherche :</span><span class="sxs-lookup"><span data-stu-id="2f0d6-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="2f0d6-105">**Emplacements de contenu et conditions de recherche**: Assurez-vous que vous avez sélectionné les emplacements de contenu et les conditions de recherche appropriés.</span><span class="sxs-lookup"><span data-stu-id="2f0d6-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="2f0d6-106">Si vous avez exécuté une recherche volumineuse (avec de nombreux emplacements), envisagez de la fractionner en plusieurs recherches.</span><span class="sxs-lookup"><span data-stu-id="2f0d6-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="2f0d6-107">**Éléments partiellement indexés**: les [éléments partiellement indexés](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) des boîtes aux lettres sont inclus dans les résultats de recherche estimés.</span><span class="sxs-lookup"><span data-stu-id="2f0d6-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="2f0d6-108">Toutefois, les éléments partiellement indexés des sites dans SharePoint et OneDrive ne sont pas inclus dans l’estimation de la recherche.</span><span class="sxs-lookup"><span data-stu-id="2f0d6-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="2f0d6-109">**Échecs de recherche**: lors de la recherche dans un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), vous pouvez obtenir des erreurs de recherche, avec des codes d’erreur comme CS008-009 et CS012-002).</span><span class="sxs-lookup"><span data-stu-id="2f0d6-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="2f0d6-110">Dans ce cas, effectuez une nouvelle tentative de recherche uniquement pour les emplacements de contenu ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="2f0d6-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="2f0d6-111">Pour plus d’informations, consultez [cet article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="2f0d6-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
