---
title: Recherche de contenu sans résultats
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816846"
---
# <a name="no-results-from-content-searchexports"></a>Aucun résultat de recherche/exportation de contenu

Les problèmes de recherche/exportation de contenu ne renvoyant aucune donnée peuvent être dus à un certain filtre de sécurité de conformité configuré par un administrateur spécifique et qui n’a pas été communiqué à tous les administrateurs.

Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine de ce problème :
1. Se connecter au Centre de sécurité et conformité PowerShell
2. Exécutez les commandes suivantes :
<br>$org = « yourdomain.com »
<br>Get-ComplianceSecurityFilter -Organization $org