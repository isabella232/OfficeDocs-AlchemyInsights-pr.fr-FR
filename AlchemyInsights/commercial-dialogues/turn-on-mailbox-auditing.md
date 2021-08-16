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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058036"
---
# <a name="turn-on-mailbox-auditing"></a>Activer l’audit des boîtes aux lettres

Pour activer l’audit de boîte aux lettres pour un utilisateur unique ou une organisation entière, exécutez les cmdlets suivantes à partir de Remote PowerShell :

- **Utilisateur unique**: Set-Mailbox -Identity « Jane Dow » -AuditEnabled $true
- **Organisation**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq « UserMailbox"} | Set-Mailbox -AuditEnabled $true

Pour plus d’informations, voir [Gérer l’audit de boîte aux lettres.](https://go.microsoft.com/fwlink/?linkid=2103668)