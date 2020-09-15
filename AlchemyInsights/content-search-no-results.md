---
title: Recherche de contenu sans résultats
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680645"
---
# <a name="no-results-from-content-searchexports"></a>Aucun résultat de la recherche/exportation de contenu

Les problèmes liés à la recherche de contenu/exportation ne renvoyant pas de données peuvent être dus à un filtre de sécurité de conformité configuré par un administrateur spécifique et ne communiquant pas avec tous les administrateurs.

Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine du problème :
1. Connexion au centre de sécurité et de conformité PowerShell
2. Exécutez l’cmdlets suivante :
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org