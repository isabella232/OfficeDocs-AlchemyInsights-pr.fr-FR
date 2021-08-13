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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926243"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Masquer Microsoft 365 groupe d’adresses dans la liste d’adresses

Pour masquer un groupe Microsoft 365 dans les listes d’adresses (LA GAL) des clients Exchange (tels que Outlook ou OWA), utilisez la commande suivante dans l’shell EXO :

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pour masquer la Microsoft 365 d’être visible pour Exchange clients, utilisez la commande suivante dans l’shell EXO :

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

