---
title: Modifier l’adresse de courrier d’un groupe Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819042"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="870b1-102">Modifier l’adresse de courrier d’un groupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="870b1-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="870b1-103">Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 à l’aide du centre d’administration.</span><span class="sxs-lookup"><span data-stu-id="870b1-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="870b1-104">Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.</span><span class="sxs-lookup"><span data-stu-id="870b1-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="870b1-105">Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="870b1-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="870b1-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="870b1-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="870b1-107">Exemple :</span><span class="sxs-lookup"><span data-stu-id="870b1-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
