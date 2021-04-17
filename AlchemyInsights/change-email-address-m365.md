---
title: Modifier l’adresse de courrier d’un groupe Microsoft 365 ou Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819078"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Modifier l’adresse de courrier d’un groupe Microsoft 365 ou Microsoft Teams

Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 ou Microsoft Teams à l’aide du [Centre d’administration Microsoft 365](https://admin.microsoft.com/). Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.

Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365/Teams :

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemple :

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
