---
title: Gérer les utilisateurs synchronisés
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541986"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="385a2-102">Impossible de définir l’adresse de messagerie principale ou de modifier les attributs utilisateur</span><span class="sxs-lookup"><span data-stu-id="385a2-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="385a2-103">Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs d’utilisateur ou d’objet ne peuvent pas être modifiés à l’aide du centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="385a2-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="385a2-104">Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez la console de gestion des utilisateurs et des groupes Active Directory locale (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="385a2-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="385a2-105">Vous pouvez également modifier des attributs ou des utilisateurs pour les utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants:</span><span class="sxs-lookup"><span data-stu-id="385a2-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="385a2-106">Set-MsolUser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="385a2-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="385a2-107">Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "test user"-LastName "user"-title "Manager"-Department "HR"</span><span class="sxs-lookup"><span data-stu-id="385a2-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="385a2-108">Remove-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="385a2-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>