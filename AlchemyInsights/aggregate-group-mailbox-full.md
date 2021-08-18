---
title: NDR complète AggregateGroupMailbox reçues pour le courrier électronique envoyé Microsoft 365 groupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315908"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>NDR complète AggregateGroupMailbox reçues pour le courrier électronique envoyé Microsoft 365 groupe

Utilisez la commande EXO Shell suivante pour créer une règle de transport Exchange pour déposer silencieusement les messages électroniques envoyés à la boîte aux lettres de groupe d’agrégation :

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Remarque**: remplacez l’adresse SMTP dans **-SentTo** par l’adresse SMTP de la boîte aux lettres de groupe agrégée dans votre client. Vous pouvez obtenir l’adresse SMTP de la boîte aux lettres de groupe d’agrégation à partir de la NDR reçue.



