---
title: Déclassement des outils eDiscovery hérités
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600365"
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

- [Office 365 Advanced eDiscovery version 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Chronologie de la retraite**:
- 1er avril 2020 : vous ne serez pas en mesure de créer des recherches et des suspensions, mais vous pouvez toujours exécuter, modifier et supprimer des recherches existantes à vos propres risques. Le support Microsoft ne prend plus en charge la découverte électronique inaltérable & conservation dans le centre d’administration Exchange.

- 1er juillet 2020 : les fonctionnalités de découverte électronique inaltérable & conservations dans le centre d’administration Exchange seront mises en lecture seule. Cela signifie que vous pourrez uniquement supprimer des recherches et des suspensions existantes.

**Pour plus d’informations, voir**:

 - [Migration des recherches et des suspensions de découverte électronique héritées vers le centre de conformité Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Déclassement des outils eDiscovery hérités](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQ sur la découverte électronique inaltérable et les conservations inaltérables](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



