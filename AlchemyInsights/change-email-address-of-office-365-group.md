---
title: Modifier l’adresse de courrier d’un groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282349"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Modifier l’adresse de courrier d’un groupe Microsoft 365

Vous pouvez modifier l’adresse de courrier d’un groupe Microsoft 365 à l’aide du centre d’administration. Sélectionnez simplement le groupe et sélectionnez @edit adresse de courrier.

Vous pouvez également utiliser la commande EXO PowerShell pour modifier l’adresse SMTP principale d’un groupe Microsoft 365 :

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exemple :

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
