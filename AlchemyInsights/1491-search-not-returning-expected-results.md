---
title: 1491-Search-not-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964857"
---
# <a name="content-search-not-returning-expected-results"></a>Recherche de contenu ne retourne ne pas les résultats attendus

Lors de l’exécution de recherches de contenu à partir du centre de conformité de & sécurité pour Microsoft Office 365, vous pouvez recevoir des résultats inattendus. Prenez en compte les éléments suivants peuvent avoir une incidence sur vos résultats de recherche :

- **Emplacements de contenu et des conditions de recherche**: Vérifiez que vous avez sélectionné les emplacements appropriés de contenu et les critères de recherche. Si vous avez exécuté une recherche de grande taille (avec nombreux emplacements), pensez à diviser en plusieurs recherches.

- **Partiellement des éléments indexés**: [partiellement des éléments indexés](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) de boîtes aux lettres sont inclus dans les résultats de recherche estimés. Toutefois, des éléments indexés partiellement à partir de sites dans SharePoint et OneDrive ne sont pas inclus dans l’estimation de la recherche.

- **Échecs de recherche**: lors de la recherche d’un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), vous obtiendrez des erreurs de recherche, avec des codes d’erreur tel que CS008-009 et CS012-002). Dans ce cas, réessayez la recherche uniquement pour les emplacements de contenu ayant échoués. Consultez [cet article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pour plus d’informations.
