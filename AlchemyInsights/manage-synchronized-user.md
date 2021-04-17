---
title: Gérer l’utilisateur synchronisé
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823965"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="06d20-102">Impossible de définir l’adresse de messagerie principale, de modifier les attributs utilisateur ou de supprimer/supprimer un utilisateur synchronisé</span><span class="sxs-lookup"><span data-stu-id="06d20-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="06d20-103">Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs utilisateur ou objet ne peuvent pas être modifiés à l’aide du Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="06d20-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="06d20-104">Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez votre console de gestion des groupes et des utilisateurs Active Directory local (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="06d20-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="06d20-105">Vous pouvez également modifier des utilisateurs individuels ou des attributs pour des utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants :</span><span class="sxs-lookup"><span data-stu-id="06d20-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
