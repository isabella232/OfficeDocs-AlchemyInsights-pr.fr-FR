---
title: Impossible de modifier le nom d’utilisateur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431509"
---
# <a name="unable-to-change-username"></a>Impossible de modifier le nom d’utilisateur

Dans certains cas, les modifications d’UPN (UserPrincipalName) ne sont pas propagées dans le cloud. Vous allez peut-être recevoir des erreurs de validation dans le portail Office 365, ou vous ne pourrez pas modifier le nom d’utilisateur ou l’adresse e-mail. Pour résoudre ce problème, configurez manuellement UserPrincipalName à l’aide de cette commande PowerShell.

**Exemple : Renommer un utilisateur**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Cette commande renomme davidc@contoso.com en davidchew@contoso.com.

Pour plus d’informations, consultez [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).