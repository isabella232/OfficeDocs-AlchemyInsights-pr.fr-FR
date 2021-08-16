---
title: Impossible de modifier le nom d’utilisateur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020226"
---
# <a name="unable-to-change-username"></a>Impossible de modifier le nom d’utilisateur

Dans certains cas, les modifications d’UPN (UserPrincipalName) ne sont pas propagées dans le cloud. Vous allez peut-être recevoir des erreurs de validation dans le portail Office 365, ou vous ne pourrez pas modifier le nom d’utilisateur ou l’adresse e-mail. Pour résoudre ce problème, configurez manuellement UserPrincipalName à l’aide de cette commande PowerShell.

**Exemple : Renommer un utilisateur**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Cette commande renomme davidc@contoso.com en davidchew@contoso.com.

Pour plus d’informations, consultez [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).