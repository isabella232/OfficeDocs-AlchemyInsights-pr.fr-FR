---
title: Recherche de contenu sans résultats
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800330"
---
# <a name="no-results-from-content-searchexports"></a>Aucun résultat de la recherche/exportation de contenu

Les problèmes liés à la recherche de contenu/exportation ne renvoyant pas de données peuvent être dus à un filtre de sécurité de conformité configuré par un administrateur spécifique et ne communiquant pas avec tous les administrateurs.

Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine du problème:
1. Connexion au centre de sécurité et de conformité PowerShell
2. Exécutez l’cmdlets suivante:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org