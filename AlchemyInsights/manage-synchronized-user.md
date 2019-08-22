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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Impossible de définir l’adresse de messagerie principale ou de modifier les attributs utilisateur

Si la synchronisation d’annuaires est activée pour votre environnement, certains attributs d’utilisateur ou d’objet ne peuvent pas être modifiés à l’aide du centre d’administration Microsoft 365.

Pour gérer entièrement les utilisateurs synchronisés et tous leurs attributs, utilisez la console de gestion des utilisateurs et des groupes Active Directory locale (adsiedit. msc).  

Vous pouvez également modifier des attributs ou des utilisateurs pour les utilisateurs synchronisés à l’aide de PowerShell, comme illustré dans les exemples courants suivants: 
- Set-MsolUser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "test user"-LastName "user"-title "Manager"-Department "HR"
- Remove-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com