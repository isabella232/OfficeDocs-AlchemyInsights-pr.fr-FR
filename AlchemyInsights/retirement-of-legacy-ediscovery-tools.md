---
title: Retrait des outils eDiscovery hérités
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
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074672"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retrait des outils eDiscovery hérités

En raison des fonctionnalités eDiscovery nouvelles et améliorées du centre de conformité Microsoft 365, les outils et les commandes eDiscovery hérités suivants seront retirés dans les prochains mois :

- [EDiscovery in-Place](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) et [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) dans le centre d’administration Exchange’administration.

- Les Exchange Online cmdlets PowerShell qui In-Place eDiscovery et In-Place holds. (Ces cmdlets sont identifiées collectivement comme des cmdlets *-MailboxSearch.) Cela inclut les cmdlets suivantes :

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) dans Exchange Online PowerShell.
- Les opérations suivantes dans l’API Exchange Services Web :
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Chronologie du retrait**:
- **1er juillet 2020** Vous ne pouvez plus créer de recherches et de nouvelles recherches, mais vous pouvez exécuter, modifier et supprimer des recherches existantes à vos propres risques. Le support Microsoft ne prend plus en charge In-Place'eDiscovery &'eDiscovery dans le EAC.
    
- **Le 1er octobre 2020,** In-Place fonctionnalité eDiscovery & Holds dans leAC sera placée en mode lecture seule, afin que vous ne pouvez supprimer que les recherches et les mises en cours existantes.

**Pour plus d’informations, voir**:

 - [Migrer les recherches et les Centre de conformité Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retrait des outils eDiscovery hérités](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQ sur les In-Place eDiscovery et les In-Place de découverte électronique](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



