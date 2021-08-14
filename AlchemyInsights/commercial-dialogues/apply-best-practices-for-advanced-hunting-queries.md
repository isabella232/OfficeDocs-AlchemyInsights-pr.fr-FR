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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930131"
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
