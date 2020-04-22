---
title: Activer l’audit de boîte aux lettres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703569"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="8b472-102">Activer l’audit de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="8b472-102">Enable mailbox auditing</span></span>

<span data-ttu-id="8b472-103">Pour activer l’audit de boîte aux lettres pour un seul utilisateur ou une organisation entière, les cmdlets suivantes doivent être exécutées à distance :</span><span class="sxs-lookup"><span data-stu-id="8b472-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="8b472-104">**Utilisateur unique**</span><span class="sxs-lookup"><span data-stu-id="8b472-104">**Single User**</span></span>
  
<span data-ttu-id="8b472-105">Set-Mailbox-Identity "Jeanne Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="8b472-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="8b472-106">**Organization**</span><span class="sxs-lookup"><span data-stu-id="8b472-106">**Organization**</span></span>
  
<span data-ttu-id="8b472-107">Get-Mailbox-result-Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="8b472-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="8b472-108">En savoir plus</span><span class="sxs-lookup"><span data-stu-id="8b472-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

