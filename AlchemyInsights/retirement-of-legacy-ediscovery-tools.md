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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798547"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="05b5c-102">Retrait des outils eDiscovery hérités</span><span class="sxs-lookup"><span data-stu-id="05b5c-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="05b5c-103">Suite aux fonctionnalités eDiscovery nouvelles et améliorées du Centre de conformité Microsoft 365, les outils et les commandes eDiscovery hérités suivants seront retirés dans les prochains mois :</span><span class="sxs-lookup"><span data-stu-id="05b5c-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="05b5c-104">[EDiscovery in-place](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) et [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) dans le Centre d'administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="05b5c-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="05b5c-105">Cmdlets Exchange Online PowerShell qui prend en charge In-Place eDiscovery et In-Place holds.</span><span class="sxs-lookup"><span data-stu-id="05b5c-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="05b5c-106">(Ces cmdlets sont identifiées collectivement comme des cmdlets \*-MailboxSearch.) Cela inclut les cmdlets suivantes :</span><span class="sxs-lookup"><span data-stu-id="05b5c-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="05b5c-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="05b5c-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="05b5c-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="05b5c-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="05b5c-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="05b5c-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="05b5c-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="05b5c-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="05b5c-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) dans Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="05b5c-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="05b5c-112">Les opérations suivantes dans l'API des services web Exchange :</span><span class="sxs-lookup"><span data-stu-id="05b5c-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="05b5c-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="05b5c-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="05b5c-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="05b5c-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="05b5c-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="05b5c-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="05b5c-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="05b5c-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="05b5c-117">**Chronologie du retrait**:</span><span class="sxs-lookup"><span data-stu-id="05b5c-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="05b5c-118">**1er juillet 2020** Vous ne pouvez plus créer de recherches et de nouvelles recherches, mais vous pouvez exécuter, modifier et supprimer des recherches existantes à vos propres risques.</span><span class="sxs-lookup"><span data-stu-id="05b5c-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="05b5c-119">Le support Microsoft ne prend plus en charge In-Place'eDiscovery &'eDiscovery dans le EAC.</span><span class="sxs-lookup"><span data-stu-id="05b5c-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="05b5c-120">**Le 1er octobre 2020,** In-Place fonctionnalité eDiscovery & Holds dans leAC sera placée en mode lecture seule, afin que vous ne pouvez supprimer que les recherches et les mises en cours existantes.</span><span class="sxs-lookup"><span data-stu-id="05b5c-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="05b5c-121">**Pour plus d'informations, voir**:</span><span class="sxs-lookup"><span data-stu-id="05b5c-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="05b5c-122">Migrer les recherches et les données de découverte électronique héritées vers le Centre de conformité Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="05b5c-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="05b5c-123">Retrait des outils eDiscovery hérités</span><span class="sxs-lookup"><span data-stu-id="05b5c-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="05b5c-124">FAQ sur les In-Place eDiscovery et les In-Place de découverte électronique</span><span class="sxs-lookup"><span data-stu-id="05b5c-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



