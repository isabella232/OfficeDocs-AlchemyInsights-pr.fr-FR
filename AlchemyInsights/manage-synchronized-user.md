---
title: Gérer les utilisateurs synchronisés
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777675"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="68aca-102">Impossible de définir l’adresse de messagerie principale, de modifier les attributs utilisateur ou de supprimer/supprimer un utilisateur synchronisé</span><span class="sxs-lookup"><span data-stu-id="68aca-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="68aca-103">Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs d’utilisateur ou d’objet ne peuvent pas être modifiés à l’aide du centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68aca-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="68aca-104">Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez la console de gestion des utilisateurs et des groupes Active Directory locale (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="68aca-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="68aca-105">Vous pouvez également modifier des attributs ou des utilisateurs pour les utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants :</span><span class="sxs-lookup"><span data-stu-id="68aca-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
