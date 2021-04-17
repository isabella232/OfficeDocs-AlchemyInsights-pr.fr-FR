---
title: Instructions pour masquer/démasqueler le groupe de la liste d’adresses
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831876"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Masquer le groupe Microsoft 365 dans la liste d’adresses

Pour masquer un groupe Microsoft 365 dans les listes d’adresses des clients Exchange (comme Outlook ou OWA), utilisez la commande suivante dans l’shell EXO :

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pour masquer la visibilité du groupe Microsoft 365 pour les clients Exchange, utilisez la commande suivante dans l’shell EXO :

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

