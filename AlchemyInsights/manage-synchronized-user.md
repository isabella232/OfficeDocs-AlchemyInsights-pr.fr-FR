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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Impossible de définir l’adresse de messagerie principale, de modifier les attributs utilisateur ou de supprimer/supprimer un utilisateur synchronisé

Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs d’utilisateur ou d’objet ne peuvent pas être modifiés à l’aide du centre d’administration Microsoft 365.

Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez la console de gestion des utilisateurs et des groupes Active Directory locale (adsiedit. msc).  

Vous pouvez également modifier des attributs ou des utilisateurs pour les utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants : 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
