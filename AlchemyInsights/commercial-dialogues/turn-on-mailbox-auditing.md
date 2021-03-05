---
title: Activer l’audit des boîtes aux lettres
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464670"
---
# <a name="turn-on-mailbox-auditing"></a>Activer l’audit des boîtes aux lettres

Pour activer l’audit de boîte aux lettres pour un utilisateur unique ou une organisation entière, exécutez les cmdlets suivantes à partir de Remote PowerShell :

- **Utilisateur unique**: Set-Mailbox -Identity « Jane Dow » -AuditEnabled $true
- **Organisation**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq « UserMailbox"} | Set-Mailbox -AuditEnabled $true

Pour plus d’informations, voir [Gérer l’audit de boîte aux lettres.](https://go.microsoft.com/fwlink/?linkid=2103668)