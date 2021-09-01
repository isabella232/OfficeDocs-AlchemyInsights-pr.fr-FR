---
title: Application de la limite de réception de boîtes aux lettres
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829149"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Application de la limite de réception de boîtes aux lettres

Microsoft a récemment commencé à appliquer le seuil par boîte aux lettres de 3 600 messages par heure. Pour plus d’informations, voir [Limites d’Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Les boîtes aux lettres Microsoft 365 qui reçoivent plus de 3 600 messages en une heure sont limitées pendant les 60 minutes suivantes. 

En outre, la limite de paires expéditeur-destinataire (SRP) qui bloque les messages reçus par une boîte aux lettres Microsoft 365 d’un expéditeur spécifique est appliquée. Si un expéditeur unique envoie plus de 33 % du seuil total ou 1 200 messages par heure de déploiement à un destinataire spécifique, la limite SRP démarre et la boîte aux lettres n’accepte plus les messages de cet expéditeur. Notez que :

- Cette limite s’appliquera aux e-mails reçus d’autres clients, locaux ou expéditeurs Internet.
- La remise du courrier électronique à la boîte aux lettres est bloquée pendant les 60 minutes suivantes. 
- Les expéditeurs de ces boîtes aux lettres reçoivent une note de non-remise (5.2.121 ou 5.2.122) indiquant que la boîte aux lettres a dépassé le seuil de remise maximal. Intra-client (courrier au sein du même client) continue d’être remis.
- Lorsque la limite SRP est appliquée, la boîte aux lettres de réception continue d’accepter les messages provenant d’autres expéditeurs.

Les administrateurs peuvent surveiller l’activité actuelle des boîtes aux lettres en accédant à un nouveau rapport et à des informations dans le Centre d’administration Exchange appelé « Boîtes aux lettres dépassant les limites de réception ». Les informations apparaissent uniquement si un client a des boîtes aux lettres incriminées, alors que le rapport apparaît toujours dans le tableau de bord mais est vide, sauf si un client a des boîtes aux lettres incriminées.

Pour plus d’informations sur les limites de réception d’informations, voir [Boîtes aux lettres dépassant les limites de réception dans le nouveau EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Pour plus d’informations sur le rapport de dépassement des limites de réception, voir [Boîtes aux lettres dépassant le rapport des limites de réception dans le nouveau EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).