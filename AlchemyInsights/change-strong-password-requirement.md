---
title: Modifier l'exigence d'un mot de passe fort
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818466"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="e8709-102">Modifier l'exigence de mot de passe fort</span><span class="sxs-lookup"><span data-stu-id="e8709-102">Change strong password requirement</span></span>

<span data-ttu-id="e8709-103">Microsoft requiert des mots de passe forts par défaut.</span><span class="sxs-lookup"><span data-stu-id="e8709-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="e8709-104">À l'aide de PowerShell, vous pouvez désactiver les mots de passe forts pour des utilisateurs spécifiques à l'aide des commandes ci-après :</span><span class="sxs-lookup"><span data-stu-id="e8709-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="e8709-105">Pour désactiver les mots de passe forts pour tous les utilisateurs, utilisez :</span><span class="sxs-lookup"><span data-stu-id="e8709-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="e8709-106">Plus d'informations sur la stratégie de mot de passe</span><span class="sxs-lookup"><span data-stu-id="e8709-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="e8709-107">Comment se connecter à Microsoft 365 avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="e8709-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="e8709-108">Plus d'informations sur les commandes PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="e8709-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
