---
title: Activer l’audit de boîte aux lettres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500280"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="23782-102">Activer l’audit de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="23782-102">Enable mailbox auditing</span></span>

<span data-ttu-id="23782-103">Pour activer l’audit de boîte aux lettres pour un utilisateur unique ou un ensemble de l’organisation, les cmdlets suivantes doit être exécutées à partir de PowerShell à distance :</span><span class="sxs-lookup"><span data-stu-id="23782-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="23782-104">**Utilisateur unique**</span><span class="sxs-lookup"><span data-stu-id="23782-104">**Single User**</span></span>
  
<span data-ttu-id="23782-105">Set-Mailbox - Identity « Jane Dow » - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="23782-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="23782-106">**Organisation**</span><span class="sxs-lookup"><span data-stu-id="23782-106">**Organization**</span></span>
  
<span data-ttu-id="23782-107">Get-Mailbox - ResultSize Unlimited - filtre {RecipientTypeDetails - eq « UserMailbox »} | Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="23782-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="23782-108">En savoir plus</span><span class="sxs-lookup"><span data-stu-id="23782-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

