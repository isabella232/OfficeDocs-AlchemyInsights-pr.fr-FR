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
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451398"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Impossible de définir l’adresse de messagerie principale, de modifier les attributs utilisateur ou de supprimer/supprimer un utilisateur synchronisé

Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs d’utilisateur ou d’objet ne peuvent pas être modifiés à l’aide du centre d’administration Microsoft 365.

Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez la console de gestion des utilisateurs et des groupes Active Directory locale (adsiedit. msc).  

Vous pouvez également modifier des attributs ou des utilisateurs pour les utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants :

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
