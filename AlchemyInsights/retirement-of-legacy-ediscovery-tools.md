---
title: Déclassement des outils eDiscovery hérités
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727781"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Déclassement des outils eDiscovery hérités

À la suite de la nouvelle fonctionnalité eDiscovery améliorée dans le centre de conformité Microsoft 365, les outils eDiscovery hérités et cmdlets suivants seront supprimés au cours des prochains mois :

- [Découverte électronique inaltérable](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) et [conservation](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) inaltérable dans le centre d’administration Exchange.

- Les cmdlets Exchange Online PowerShell qui prennent en charge la découverte électronique inaltérable et les conservations inaltérables. (Ces cmdlets sont collectivement identifiées en tant que cmdlets *-MailboxSearch.) Cela inclut les applets de commande suivantes :

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) dans Exchange Online PowerShell.
- Les opérations suivantes dans l’API des services Web Exchange :
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Chronologie de la retraite**:
- **1er juillet 2020** Vous ne pouvez plus créer de nouvelles recherches et suspensions, mais vous pouvez exécuter, modifier et supprimer des recherches existantes à vos propres risques. Le support Microsoft ne prend plus en charge la découverte électronique inaltérable & conservation dans le centre d’administration Exchange.
    
- **1er octobre 2020** & de découverte électronique inaltérable les fonctionnalités du centre d’administration Exchange seront mises en lecture seule, de sorte que vous ne pouvez supprimer que les recherches et les suspensions existantes.

**Pour plus d’informations, voir**:

 - [Migration des recherches et des suspensions de découverte électronique héritées vers le centre de conformité Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retrait des outils eDiscovery hérités](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQ sur la découverte électronique inaltérable et les conservations inaltérables](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



