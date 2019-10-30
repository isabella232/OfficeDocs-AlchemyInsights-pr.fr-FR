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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768918"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Masquer le groupe Office 365 de la liste d’adresses (LAG)

Pour masquer un groupe Office 365 dans les listes d’adresses (LAG) des clients Exchange (par exemple, Outlook ou OWA), utilisez la commande suivante dans l’environnement de EXO :

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pour masquer le groupe Office 365 de façon à ce qu’il soit visible pour les clients Exchange, utilisez la commande suivante dans EXO Shell :

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

