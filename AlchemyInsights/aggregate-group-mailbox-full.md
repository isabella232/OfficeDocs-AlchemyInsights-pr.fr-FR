---
title: Rapport de non-remise complet AggregateGroupMailbox reçu pour les messages envoyés au groupe Microsoft 365
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715699"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Rapport de non-remise complet AggregateGroupMailbox reçu pour les messages envoyés au groupe Microsoft 365

Utilisez la commande EXO Shell suivante pour créer une règle de transport Exchange afin de supprimer silencieusement les messages électroniques envoyés à la boîte aux lettres de groupe d’agrégats :

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Remplacez l’adresse SMTP dans **-SentTo** par l’adresse SMTP de la boîte aux lettres de groupe d’agrégation de votre client. Vous pouvez obtenir l’adresse SMTP de la boîte aux lettres de groupe d’agrégation à partir de la notification d’inversion reçue.



