---
title: Impossible de modifier le nom d’utilisateur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798662"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="4fe43-102">Impossible de modifier le nom d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="4fe43-102">Unable to change UserName</span></span>

<span data-ttu-id="4fe43-103">Dans certains cas, les modifications d’UPN (UserPrincipalName) ne sont pas propagées dans le cloud.</span><span class="sxs-lookup"><span data-stu-id="4fe43-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="4fe43-104">Vous allez peut-être recevoir des erreurs de validation dans le portail Office 365, ou vous ne pourrez pas modifier le nom d’utilisateur ou l’adresse e-mail.</span><span class="sxs-lookup"><span data-stu-id="4fe43-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="4fe43-105">Pour résoudre ce problème, configurez manuellement UserPrincipalName à l’aide de cette commande PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4fe43-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="4fe43-106">**Exemple : Renommer un utilisateur**</span><span class="sxs-lookup"><span data-stu-id="4fe43-106">**Example: Rename a user**</span></span>

<span data-ttu-id="4fe43-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="4fe43-107">PowerShellCopy</span></span>

<span data-ttu-id="4fe43-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="4fe43-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="4fe43-109">Cette commande renomme davidc@contoso.com en davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4fe43-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="4fe43-110">Pour plus d’informations, consultez [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="4fe43-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>