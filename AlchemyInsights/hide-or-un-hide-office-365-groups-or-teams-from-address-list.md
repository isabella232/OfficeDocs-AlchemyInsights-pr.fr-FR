---
title: Masquer ou afficher les groupes ou équipes Office 365 dans la liste d’adresses
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811454"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="ad76d-102">Masquer ou afficher les groupes ou équipes Office 365 dans la liste d’adresses</span><span class="sxs-lookup"><span data-stu-id="ad76d-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="ad76d-103">Utiliser la commande EXO PowerShell suivante pour masquer ou afficher les groupes/équipes Office 365 dans les listes d’adresses (GAL) des clients Exchange (Outlook, OWA) :</span><span class="sxs-lookup"><span data-stu-id="ad76d-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="ad76d-104">Utiliser la commande EXO PowerShell suivante pour masquer ou afficher les groupes/équipes Office 365 des clients Exchange (Outlook, OWA) :</span><span class="sxs-lookup"><span data-stu-id="ad76d-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="ad76d-105">Pour obtenir des instructions détaillées, voir [Masquer les groupes Office 365 dans la liste d’adresses globale et des clients Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="ad76d-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
