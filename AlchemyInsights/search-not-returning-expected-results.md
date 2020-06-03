---
title: 1491-ne pas renvoyer-résultats attendus
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510570"
---
# <a name="content-search-not-returning-expected-results"></a>Recherche de contenu ne renvoyant pas les résultats attendus

Lors de l’exécution de recherches de contenu à partir du centre de conformité & Microsoft 365 Security, vous pouvez recevoir des résultats de recherche inattendus. Tenez compte des éléments suivants qui peuvent avoir une incidence sur vos résultats de recherche :

- **Emplacements de contenu et conditions de recherche**: Assurez-vous que vous avez sélectionné les emplacements de contenu et les conditions de recherche appropriés. Si vous avez exécuté une recherche volumineuse (avec de nombreux emplacements), envisagez de la fractionner en plusieurs recherches.

- **Éléments partiellement indexés**: les [éléments partiellement indexés](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) des boîtes aux lettres sont inclus dans les résultats de recherche estimés. Toutefois, les éléments partiellement indexés des sites dans SharePoint et OneDrive ne sont pas inclus dans l’estimation de la recherche.

- **Échecs de recherche**: lors de la recherche dans un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), vous pouvez obtenir des erreurs de recherche, avec des codes d’erreur comme CS008-009 et CS012-002). Dans ce cas, effectuez une nouvelle tentative de recherche uniquement pour les emplacements de contenu ayant échoué. Pour plus d’informations, consultez [cet article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
