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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088394"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Masquer ou afficher les groupes ou équipes Office 365 dans la liste d’adresses

Utiliser la commande EXO PowerShell suivante pour masquer ou afficher les groupes/équipes Office 365 dans les listes d’adresses (GAL) des clients Exchange (Outlook, OWA) :

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Utiliser la commande EXO PowerShell suivante pour masquer ou afficher les groupes/équipes Office 365 des clients Exchange (Outlook, OWA) :

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Pour obtenir des instructions détaillées, voir [Masquer les groupes Office 365 dans la liste d’adresses globale et des clients Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
