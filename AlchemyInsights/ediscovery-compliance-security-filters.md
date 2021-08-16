---
title: Aucun résultat renvoyé pendant la recherche/exportation de contenu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101264"
---
# <a name="no-results-returned-during-content-searchexport"></a>Aucun résultat renvoyé pendant la recherche/exportation de contenu

Si vous rencontrez des problèmes avec les scénarios eDiscovery suivants :

- La recherche/exportation de contenu ne renvoie aucune donnée ou donnée inattendue
- Échec de la recherche ou de l’exportation eDiscovery

Cela peut être dû à certains filtres de sécurité de conformité qui ont été configurés par un administrateur spécifique et qui n’ont pas été communiquées à tous les administrateurs.

Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine de ces problèmes :

1. Connecter centre de sécurité et conformité PowerShell
2. Exécutez les commandes suivantes :

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Pour plus d’informations sur les filtres de sécurité de la conformité, voir Filtrage des [autorisations pour la recherche de contenu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
