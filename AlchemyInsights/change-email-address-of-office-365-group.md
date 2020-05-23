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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282349"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="d9578-102">Modifier l’adresse de courrier d’un groupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d9578-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="d9578-103">Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 à l’aide du centre d’administration.</span><span class="sxs-lookup"><span data-stu-id="d9578-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="d9578-104">Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.</span><span class="sxs-lookup"><span data-stu-id="d9578-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="d9578-105">Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="d9578-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="d9578-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="d9578-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="d9578-107">Exemple :</span><span class="sxs-lookup"><span data-stu-id="d9578-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
