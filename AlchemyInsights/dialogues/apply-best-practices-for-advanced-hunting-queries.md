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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568619"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Appliquer les meilleures pratiques pour les requêtes de recherche avancées

Pour obtenir des résultats plus rapidement et éviter les délai d’accès lors de l’exécution de requêtes complexes, appliquez les meilleures pratiques ci-après :

- Lorsque vous essayez de nouvelles requêtes, utilisez toujours une limite pour éviter d’obtenir des jeux de résultats extrêmement grands. Utilisez également cette étape pour effectuer une évaluation initiale de la taille `count` du jeu de résultats.
- Utilisez tout d’abord les filtres de temps. Dans l’idéal, limitez vos requêtes à sept jours.
- Au début d’une requête, juste après le filtre d’heure, ajoutez les filtres censés supprimer la plupart des données.
- Lorsque vous recherchez des jetons complets, utilisez `has` l’opérateur plutôt que `contains` .
- Exécutez une recherche sur une colonne spécifique plutôt que sur toutes les colonnes.
- Lorsque vous joignez des tables, spécifiez d’abord la table avec moins de lignes.
- `project` uniquement les colonnes nécessaires des tables que vous avez jointes.

Pour en savoir plus, consultez les meilleures pratiques [en matière de requête de recherche avancée.](https://go.microsoft.com/fwlink/?linkid=2144812)
