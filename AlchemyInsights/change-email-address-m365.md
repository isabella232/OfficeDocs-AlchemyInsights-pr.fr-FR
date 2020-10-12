---
title: Modifier l’adresse de courrier d’un groupe Microsoft 365
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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416694"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Modifier l’adresse de courrier d’un groupe Microsoft 365

Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 à l’aide du centre d’administration. Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.

Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365 :

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemple :

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
