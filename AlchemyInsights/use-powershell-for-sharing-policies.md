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
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998464"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Utiliser PowerShell pour les stratégies de partage et les relations d’organisation


Pour les relations d’organisation, veuillez consulter les informations de syntaxe et de paramètre détaillées pour les éléments suivants : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) et [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Pour créer une stratégie de partage, utilisez [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Pour [appliquer une stratégie de partage à une boîte aux lettres ou à un utilisateur](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), vous devez utiliser une combinaison de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) et [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) avec la stratégie nouvellement créée. Pour [modifier, désactiver ou supprimer une stratégie de partage](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), vous devez utiliser [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) et [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Pour une compréhension complète de ce sujet, veuillez consulter :**

[Partage dans Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)