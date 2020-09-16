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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="00b88-102">Déclassement des outils eDiscovery hérités</span><span class="sxs-lookup"><span data-stu-id="00b88-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="00b88-103">À la suite de la nouvelle fonctionnalité eDiscovery améliorée dans le centre de conformité Microsoft 365, les outils eDiscovery hérités et cmdlets suivants seront supprimés au cours des prochains mois :</span><span class="sxs-lookup"><span data-stu-id="00b88-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="00b88-104">[Découverte électronique inaltérable](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) et [conservation](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) inaltérable dans le centre d’administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="00b88-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="00b88-105">Les cmdlets Exchange Online PowerShell qui prennent en charge la découverte électronique inaltérable et les conservations inaltérables.</span><span class="sxs-lookup"><span data-stu-id="00b88-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="00b88-106">(Ces cmdlets sont collectivement identifiées en tant que cmdlets \*-MailboxSearch.) Cela inclut les applets de commande suivantes :</span><span class="sxs-lookup"><span data-stu-id="00b88-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="00b88-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="00b88-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="00b88-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="00b88-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="00b88-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="00b88-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="00b88-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="00b88-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="00b88-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) dans Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="00b88-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="00b88-112">Les opérations suivantes dans l’API des services Web Exchange :</span><span class="sxs-lookup"><span data-stu-id="00b88-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="00b88-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="00b88-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="00b88-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="00b88-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="00b88-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="00b88-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="00b88-116">Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="00b88-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="00b88-117">**Chronologie de la retraite**:</span><span class="sxs-lookup"><span data-stu-id="00b88-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="00b88-118">**1er juillet 2020** Vous ne pouvez plus créer de nouvelles recherches et suspensions, mais vous pouvez exécuter, modifier et supprimer des recherches existantes à vos propres risques.</span><span class="sxs-lookup"><span data-stu-id="00b88-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="00b88-119">Le support Microsoft ne prend plus en charge la découverte électronique inaltérable & conservation dans le centre d’administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="00b88-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="00b88-120">**1er octobre 2020** & de découverte électronique inaltérable les fonctionnalités du centre d’administration Exchange seront mises en lecture seule, de sorte que vous ne pouvez supprimer que les recherches et les suspensions existantes.</span><span class="sxs-lookup"><span data-stu-id="00b88-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="00b88-121">**Pour plus d’informations, voir**:</span><span class="sxs-lookup"><span data-stu-id="00b88-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="00b88-122">Migration des recherches et des suspensions de découverte électronique héritées vers le centre de conformité Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="00b88-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="00b88-123">Retrait des outils eDiscovery hérités</span><span class="sxs-lookup"><span data-stu-id="00b88-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="00b88-124">FAQ sur la découverte électronique inaltérable et les conservations inaltérables</span><span class="sxs-lookup"><span data-stu-id="00b88-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



