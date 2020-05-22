---
title: Masquer ou afficher les groupes ou équipes Office 365 dans la liste d’adresses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225377"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="fb5a0-102">Masquer ou afficher les groupes ou équipes Office 365 dans la liste d’adresses</span><span class="sxs-lookup"><span data-stu-id="fb5a0-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="fb5a0-103">Utiliser la commande EXO PowerShell suivante pour masquer ou afficher les groupes/équipes Office 365 dans les listes d’adresses (GAL) des clients Exchange (Outlook, OWA) :</span><span class="sxs-lookup"><span data-stu-id="fb5a0-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="fb5a0-104">Utiliser la commande EXO PowerShell suivante pour masquer ou afficher les groupes/équipes Office 365 des clients Exchange (Outlook, OWA) :</span><span class="sxs-lookup"><span data-stu-id="fb5a0-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="fb5a0-105">Pour obtenir des instructions détaillées, voir [Masquer les groupes Office 365 dans la liste d’adresses globale et des clients Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="fb5a0-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
