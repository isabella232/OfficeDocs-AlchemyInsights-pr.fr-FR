---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052708"
---
# <a name="content-search-not-returning-expected-results"></a>Recherche de contenu ne renvoyant pas les résultats attendus

Lorsque vous exécutez des recherches de contenu à partir du centre Microsoft 365 sécurité & conformité, vous pouvez recevoir des résultats de recherche inattendus. Prenez en compte les éléments suivants qui peuvent affecter vos résultats de recherche :

- **Emplacements de contenu et conditions de** recherche : assurez-vous que vous avez sélectionné les emplacements de contenu et les conditions de recherche appropriés. Si vous avez fait une recherche de grande taille (avec de nombreux emplacements), envisagez de la fractionner en plusieurs recherches.

- **Éléments partiellement indexés**: les éléments  [partiellement indexés](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) à partir de boîtes aux lettres sont inclus dans les résultats de recherche estimés. Toutefois, les éléments partiellement indexés à partir de sites SharePoint et OneDrive ne sont pas inclus dans l’estimation de la recherche.

- Échecs de recherche : lorsque vous recherchez un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), vous pouvez obtenir des **erreurs** de recherche, avec des codes d’erreur tels que CS008-009 et CS012-002). Dans ce cas, réessayez de rechercher uniquement les emplacements de contenu qui ont échoué. Pour plus  [d’informations,](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) consultez cet article.
