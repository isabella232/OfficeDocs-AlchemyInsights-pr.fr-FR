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
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="ea6d1-102">Masquer le groupe Office 365 de la liste d’adresses (LAG)</span><span class="sxs-lookup"><span data-stu-id="ea6d1-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="ea6d1-103">Pour masquer un groupe Office 365 dans les listes d’adresses (LAG) des clients Exchange (par exemple, Outlook ou OWA), utilisez la commande suivante dans l’environnement de EXO :</span><span class="sxs-lookup"><span data-stu-id="ea6d1-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="ea6d1-104">Pour masquer le groupe Office 365 de façon à ce qu’il soit visible pour les clients Exchange, utilisez la commande suivante dans EXO Shell :</span><span class="sxs-lookup"><span data-stu-id="ea6d1-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

