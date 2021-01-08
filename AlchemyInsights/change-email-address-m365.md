---
title: Modifier l’adresse de courrier d’un groupe Microsoft 365 ou Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756555"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Modifier l’adresse de courrier d’un groupe Microsoft 365 ou Microsoft Teams

Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 ou Microsoft Teams à l’aide du [Centre d’administration Microsoft 365](https://admin.microsoft.com/). Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.

Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365/Teams :

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemple :

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
