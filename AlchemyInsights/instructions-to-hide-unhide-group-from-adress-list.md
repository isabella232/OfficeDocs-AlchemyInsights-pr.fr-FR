---
title: Instructions pour masquer/afficher le groupe de la liste d’adresses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908342"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Masquer le groupe Microsoft 365 de la liste d’adresses (LAG)

Pour masquer un groupe Microsoft 365 de listes d’adresses (LAG) de clients Exchange (par exemple, Outlook ou OWA), utilisez la commande suivante dans EXO Shell :

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pour masquer le groupe Microsoft 365 de façon à ce qu’il soit visible pour les clients Exchange, utilisez la commande suivante dans EXO Shell :

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

