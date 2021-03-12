---
title: Appliquer les meilleures pratiques pour les requêtes de recherche avancées
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736859"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="be796-102">Appliquer les meilleures pratiques pour les requêtes de recherche avancées</span><span class="sxs-lookup"><span data-stu-id="be796-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="be796-103">Pour obtenir des résultats plus rapidement et éviter les délai d’accès lors de l’exécution de requêtes complexes, appliquez les meilleures pratiques ci-après :</span><span class="sxs-lookup"><span data-stu-id="be796-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="be796-104">Lorsque vous essayez de nouvelles requêtes, utilisez toujours une limite pour éviter d’obtenir des jeux de résultats extrêmement grands.</span><span class="sxs-lookup"><span data-stu-id="be796-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="be796-105">Utilisez également cette étape pour effectuer une évaluation initiale de la taille `count` du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="be796-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="be796-106">Utilisez tout d’abord les filtres de temps.</span><span class="sxs-lookup"><span data-stu-id="be796-106">Use time filters first.</span></span> <span data-ttu-id="be796-107">Dans l’idéal, limitez vos requêtes à sept jours.</span><span class="sxs-lookup"><span data-stu-id="be796-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="be796-108">Au début d’une requête, juste après le filtre d’heure, ajoutez les filtres censés supprimer la plupart des données.</span><span class="sxs-lookup"><span data-stu-id="be796-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="be796-109">Lorsque vous recherchez des jetons complets, utilisez `has` l’opérateur plutôt que `contains` .</span><span class="sxs-lookup"><span data-stu-id="be796-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="be796-110">Exécutez une recherche sur une colonne spécifique plutôt que sur toutes les colonnes.</span><span class="sxs-lookup"><span data-stu-id="be796-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="be796-111">Lorsque vous joignez des tables, spécifiez d’abord la table avec moins de lignes.</span><span class="sxs-lookup"><span data-stu-id="be796-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="be796-112">`project` uniquement les colonnes nécessaires des tables que vous avez jointes.</span><span class="sxs-lookup"><span data-stu-id="be796-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="be796-113">Pour en savoir plus, consultez les meilleures pratiques [en matière de requête de recherche avancée.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="be796-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
