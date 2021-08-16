---
title: 'Pour configurer la réponse automatique pour tous les messages électroniques envoyés à un groupe Microsoft 365 :'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 3ed937d38627c1089c9203550498ce7b21ce01c0c5a2deea7326f8057f5338d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036130"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Pour configurer la réponse automatique pour tous les messages électroniques envoyés à un groupe Microsoft 365 :

**Connectez-vous à PowerShell EXO à l’aide d’un compte d’administrateur client et utilisez les commandes suivantes** :

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> Modifiez **groupmailbox** par un nom de groupe sur lequel vous voulez configurer la réponse automatique.

