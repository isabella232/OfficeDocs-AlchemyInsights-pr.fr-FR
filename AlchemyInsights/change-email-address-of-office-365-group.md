---
title: Modifier l’adresse de courrier d’un groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580655"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="4493a-102">Modifier l’adresse de courrier d’un groupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4493a-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="4493a-103">Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 à l’aide du centre d’administration.</span><span class="sxs-lookup"><span data-stu-id="4493a-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="4493a-104">Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.</span><span class="sxs-lookup"><span data-stu-id="4493a-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="4493a-105">Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="4493a-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="4493a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="4493a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="4493a-107">Exemple :</span><span class="sxs-lookup"><span data-stu-id="4493a-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
