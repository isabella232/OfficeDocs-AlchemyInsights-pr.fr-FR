---
title: Activer l’audit de boîte aux lettres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736251"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="cfd8d-102">Activer l’audit de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="cfd8d-102">Enable mailbox auditing</span></span>

<span data-ttu-id="cfd8d-103">Pour activer l’audit de boîte aux lettres pour un seul utilisateur ou une organisation entière, les cmdlets suivantes doivent être exécutées à distance :</span><span class="sxs-lookup"><span data-stu-id="cfd8d-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="cfd8d-104">**Utilisateur unique**</span><span class="sxs-lookup"><span data-stu-id="cfd8d-104">**Single User**</span></span>
  
<span data-ttu-id="cfd8d-105">Set-Mailbox-Identity "Jeanne Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="cfd8d-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="cfd8d-106">**Organization**</span><span class="sxs-lookup"><span data-stu-id="cfd8d-106">**Organization**</span></span>
  
<span data-ttu-id="cfd8d-107">Get-Mailbox-result-Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="cfd8d-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="cfd8d-108">En savoir plus</span><span class="sxs-lookup"><span data-stu-id="cfd8d-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

