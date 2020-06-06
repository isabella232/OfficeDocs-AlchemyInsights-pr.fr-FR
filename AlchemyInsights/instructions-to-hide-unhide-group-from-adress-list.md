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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580007"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Masquer le groupe Microsoft 365 de la liste d’adresses (LAG)

Pour masquer un groupe Microsoft 365 dans les listes d’adresses (LAG) des clients Exchange (par exemple, Outlook ou OWA), utilisez la commande suivante dans l’environnement de EXO :

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pour masquer le groupe Microsoft 365 de façon à ce qu’il soit visible pour les clients Exchange, utilisez la commande suivante dans EXO Shell :

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

