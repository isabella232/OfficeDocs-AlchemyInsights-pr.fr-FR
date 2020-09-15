---
title: Instructions pour masquer/afficher le groupe de la liste d’adresses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663007"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Masquer le groupe Microsoft 365 de la liste d’adresses (LAG)

Pour masquer un groupe Microsoft 365 dans les listes d’adresses (LAG) des clients Exchange (par exemple, Outlook ou OWA), utilisez la commande suivante dans l’environnement de EXO :

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pour masquer le groupe Microsoft 365 de façon à ce qu’il soit visible pour les clients Exchange, utilisez la commande suivante dans EXO Shell :

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

