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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="2dfbe-102">Masquer le groupe Microsoft 365 de la liste d’adresses (LAG)</span><span class="sxs-lookup"><span data-stu-id="2dfbe-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="2dfbe-103">Pour masquer un groupe Microsoft 365 dans les listes d’adresses (LAG) des clients Exchange (par exemple, Outlook ou OWA), utilisez la commande suivante dans l’environnement de EXO :</span><span class="sxs-lookup"><span data-stu-id="2dfbe-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="2dfbe-104">Pour masquer le groupe Microsoft 365 de façon à ce qu’il soit visible pour les clients Exchange, utilisez la commande suivante dans EXO Shell :</span><span class="sxs-lookup"><span data-stu-id="2dfbe-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

