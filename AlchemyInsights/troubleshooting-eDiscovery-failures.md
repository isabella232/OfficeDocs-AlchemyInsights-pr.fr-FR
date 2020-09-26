---
title: 1490-dépannage-échecs de découverte électronique
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277837"
---
# <a name="troubleshoot-content-search-errors"></a>Résoudre les erreurs de recherche de contenu

Rencontrez-vous des problèmes avec la recherche de contenu ou lorsque vous exportez des résultats de recherche ?

Par exemple, avez-vous reçu les informations suivantes lors de l’exécution des recherches ?

- Erreurs CS008 ou CS012

- Erreurs d’occupation/de délai d’attente du serveur

- Une erreur d’application s’est produite

Ou lorsque vous recherchez ou exportez des résultats à partir d’un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), recevez-vous des erreurs d’exportation ?

Pour ces types d’erreurs, essayez de relancer la recherche pour les emplacements de contenu ayant échoué. Pour plus d’informations, consultez  [cet article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Si vous exportez plus de 100 000 boîtes aux lettres, vous devez utiliser le PowerShell suivant pour télécharger les résultats de l’exportation :  [Exporter les résultats de plus de 100 000 boîtes aux lettres](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
