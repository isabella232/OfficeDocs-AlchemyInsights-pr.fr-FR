---
title: Aucun résultat renvoyé lors de la recherche/exportation de contenu
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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666643"
---
# <a name="no-results-returned-during-content-searchexport"></a>Aucun résultat renvoyé lors de la recherche/exportation de contenu

Si vous rencontrez des problèmes avec les scénarios eDiscovery suivants :

- Recherche/exportation de contenu ne renvoie aucune donnée ni aucune donnée inattendue
- échec de la recherche eDiscovery ou de l’exportation

Cela peut être dû à certains filtres de sécurité de conformité qui ont été configurés par un administrateur spécifique et qui n’ont pas été communiqués à tous les administrateurs.

Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité susceptibles d’être à l’origine des problèmes suivants :

1. Connexion au centre de sécurité et de conformité PowerShell
2. Exécutez l’cmdlets suivante :

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Pour plus d’informations sur les filtres de sécurité de conformité, consultez la rubrique [filtrage des autorisations pour la recherche de contenu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
