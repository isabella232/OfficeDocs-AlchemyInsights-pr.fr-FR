---
title: Masquer ou afficher les groupes ou équipes Office 365 dans la liste d’adresses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782325"
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
