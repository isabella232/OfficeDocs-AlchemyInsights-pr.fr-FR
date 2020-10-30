---
title: Modifier les conditions de mot de passe fort
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804421"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="bd72f-102">Modifier les conditions de mot de passe fort</span><span class="sxs-lookup"><span data-stu-id="bd72f-102">Change strong password requirement</span></span>

<span data-ttu-id="bd72f-103">Par défaut, Microsoft requiert des mots de passe forts.</span><span class="sxs-lookup"><span data-stu-id="bd72f-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="bd72f-104">À l’aide de PowerShell, vous pouvez désactiver les mots de passe forts pour des utilisateurs spécifiques à l’aide des commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="bd72f-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="bd72f-105">Pour désactiver les mots de passe forts pour tous les utilisateurs, utilisez :</span><span class="sxs-lookup"><span data-stu-id="bd72f-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="bd72f-106">Plus d’informations sur la stratégie de mot de passe</span><span class="sxs-lookup"><span data-stu-id="bd72f-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="bd72f-107">Comment se connecter à Microsoft 365 avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd72f-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="bd72f-108">Plus d’informations sur les commandes MsolUser de PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd72f-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
