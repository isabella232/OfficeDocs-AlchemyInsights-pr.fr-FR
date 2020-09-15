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
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681870"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="a4ebe-102">Modifier les conditions de mot de passe fort</span><span class="sxs-lookup"><span data-stu-id="a4ebe-102">Change strong password requirement</span></span>

<span data-ttu-id="a4ebe-103">Par défaut, Microsoft requiert des mots de passe forts.</span><span class="sxs-lookup"><span data-stu-id="a4ebe-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="a4ebe-104">À l’aide de PowerShell, vous pouvez désactiver les mots de passe forts pour des utilisateurs spécifiques à l’aide de cette commande :</span><span class="sxs-lookup"><span data-stu-id="a4ebe-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="a4ebe-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="a4ebe-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="a4ebe-106">Plus d’informations sur la stratégie de mot de passe</span><span class="sxs-lookup"><span data-stu-id="a4ebe-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="a4ebe-107">Comment se connecter à Microsoft 365 avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="a4ebe-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="a4ebe-108">Plus d’informations sur les commandes MsolUser de PowerShell</span><span class="sxs-lookup"><span data-stu-id="a4ebe-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
