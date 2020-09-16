---
title: Micro-retards ou limitations dans Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743912"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="12b10-102">Micro-retards ou limitations dans Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="12b10-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="12b10-103">Vous pouvez remarquer des avertissements ou des retards de type « Micro-retard appliqué » lorsque vous exécutez des scripts et des applets de commande dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="12b10-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="12b10-104">Voici deux suggestions relatives à ce problème :</span><span class="sxs-lookup"><span data-stu-id="12b10-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="12b10-105">Vous voudrez peut-être essayer d’utiliser le [module Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), qui inclut des applets de commande reposant sur l’API REST et qui sont considérablement plus performantes.</span><span class="sxs-lookup"><span data-stu-id="12b10-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="12b10-106">Il peut s’agir de la solution idéale pour un grand nombre de d’applets de commande Get fréquemment utilisées.</span><span class="sxs-lookup"><span data-stu-id="12b10-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="12b10-107">Si vous avez besoin d’utiliser des applets de commande qui ne sont pas encore couvertes dans le module v2, veuillez consulter [Exécution d’applets de commande PowerShell pour un grand nombre d’utilisateurs dans Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), qui évoque la façon de contourner des limitations attendues de PowerShell dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="12b10-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
