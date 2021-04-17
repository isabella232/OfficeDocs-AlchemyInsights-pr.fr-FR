---
title: Utiliser PowerShell pour les stratégies de partage et les relations d’organisation
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
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826053"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Utiliser PowerShell pour les stratégies de partage et les relations d’organisation


Pour les relations d’organisation, veuillez consulter les informations de syntaxe et de paramètre détaillées pour les éléments suivants : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) et [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Pour créer une stratégie de partage, utilisez [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Pour [appliquer une stratégie de partage à une boîte aux lettres ou à un utilisateur](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), vous devez utiliser une combinaison de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) et [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) avec la stratégie nouvellement créée. Pour [modifier, désactiver ou supprimer une stratégie de partage](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), vous devez utiliser [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) et [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Pour une compréhension complète de ce sujet, veuillez consulter :**

[Partage dans Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)