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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114776"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Impossible de définir l’adresse de messagerie principale, de modifier les attributs utilisateur ou de supprimer/supprimer un utilisateur synchronisé

Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs utilisateur ou objet ne peuvent pas être modifiés à l’aide Centre d’administration Microsoft 365.

Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez votre console de gestion des groupes et des utilisateurs Active Directory local (adsiedit.msc).  

Vous pouvez également modifier des utilisateurs individuels ou des attributs pour des utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants :

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
