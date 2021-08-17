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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058000"
---
# <a name="no-results-from-content-searchexports"></a>Aucun résultat de recherche/exportation de contenu

Les problèmes de recherche/exportation de contenu ne renvoyant aucune donnée peuvent être dus à un certain filtre de sécurité de conformité configuré par un administrateur spécifique et qui n’a pas été communiqué à tous les administrateurs.

Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine de ce problème :
1. Connecter centre de sécurité et conformité PowerShell
2. Exécutez les commandes suivantes :
<br>$org = « yourdomain.com »
<br>Get-ComplianceSecurityFilter -Organization $org