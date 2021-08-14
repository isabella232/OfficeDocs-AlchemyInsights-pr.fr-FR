---
title: NDR complète AggregateGroupMailbox reçues pour les messages envoyés Microsoft 365 groupe
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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951851"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>NDR complète AggregateGroupMailbox reçues pour les messages envoyés Microsoft 365 groupe

Utilisez la commande EXO Shell suivante pour créer une règle de transport Exchange pour déposer silencieusement les messages électroniques envoyés à la boîte aux lettres de groupe d’agrégation :

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Remplacez l’adresse SMTP dans **-SentTo** par l’adresse SMTP de la boîte aux lettres de groupe agrégée dans votre client. Vous pouvez obtenir l’adresse SMTP de la boîte aux lettres de groupe d’agrégation à partir de la NDR reçue.



