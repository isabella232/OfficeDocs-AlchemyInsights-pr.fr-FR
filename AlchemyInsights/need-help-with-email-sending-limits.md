---
title: Vous avez besoin d’aide sur les limites d’envoi des e-mails ?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836277"
---
# <a name="need-help-with-email-sending-limits"></a>Vous avez besoin d’aide sur les limites d’envoi des e-mails ?

Vous trouverez ci-dessous les **limites d’envoi par la conception** appliquées dans le service. Vous trouverez plus d’informations sur ces limites [ici](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- Pour décourager la livraison de messages en bloc non sollicités, nous appliquons des **limites de débit maximal pour les destinataires par utilisateur à tous les messages internes et sortants**. Pour toutes les références SKU, cette limite est de **10 000 destinataires par jour**.  Les clients qui doivent envoyer légitimement des e-mails commerciaux en nombre (par exemple, des bulletins d’information des clients) doivent faire appel à des fournisseurs tiers spécialisés dans ces services.
    - **Remarque** : une fois la limite de débit maximale pour tous les destinataires atteinte, il est impossible d’envoyer des messages à partir de la boîte aux lettres tant que le nombre de destinataires des messages envoyés au cours des dernières 24 heures n’est pas redescendu en dessous de la limite. L’utilisateur ne pourra pas envoyer de messages d’ici là.
- La limite de débit de **30 messages par minute** est appliquée sur toutes les références SKU. Cet élément détermine le nombre de messages qu'un utilisateur peut envoyer à partir de son compte Exchange Online pendant une période spécifiée.
- Le **nombre maximal de destinataires autorisés dans les champs À, Cc et Cci** pour un seul e-mail sur toutes les références SKU est de **1000**. Pour personnaliser cette limite, rendez-vous [ici](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
