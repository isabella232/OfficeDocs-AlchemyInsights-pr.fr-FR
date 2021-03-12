---
title: Utiliser PowerShell pour les stratégies de partage et les relations d’organisation
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
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709464"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="b6f1c-102">Utiliser PowerShell pour les stratégies de partage et les relations d’organisation</span><span class="sxs-lookup"><span data-stu-id="b6f1c-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="b6f1c-103">Pour les relations d’organisation, veuillez consulter les informations de syntaxe et de paramètre détaillées pour les éléments suivants : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) et [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="b6f1c-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="b6f1c-104">Pour créer une stratégie de partage, utilisez [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b6f1c-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="b6f1c-105">Pour [appliquer une stratégie de partage à une boîte aux lettres ou à un utilisateur](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), vous devez utiliser une combinaison de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) et [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) avec la stratégie nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="b6f1c-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="b6f1c-106">Pour [modifier, désactiver ou supprimer une stratégie de partage](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), vous devez utiliser [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) et [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b6f1c-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="b6f1c-107">**Pour une compréhension complète de ce sujet, veuillez consulter :**</span><span class="sxs-lookup"><span data-stu-id="b6f1c-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="b6f1c-108">Partage dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b6f1c-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)