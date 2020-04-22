---
title: Courrier électronique sortant vers le dossier courrier indésirable
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761166"
---
# <a name="outbound-email-to-junk-email-folder"></a>Courrier électronique sortant vers le dossier courrier indésirable

Si vous constatez que les messages sortants sont marqués comme courrier indésirable, procédez comme suit :

- Si vous ne l’avez pas encore fait, envisagez de [configurer les notifications de stratégie de courrier indésirable sortant](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).

- Utilisez le [suivi des messages](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) pour voir si le message sortant a la valeur de l’événement **courrier indésirable** avec les détails supplémentaires : **utiliser un pool de remise à risque élevé**.

  Pour ces messages, vérifiez le contenu du message pour voir ce qui peut être considéré comme du courrier indésirable. Par exemple, les signatures peuvent parfois causer des problèmes à de nombreux utilisateurs.

  Si vous avez plusieurs exemples de messages sortants légitimes marqués comme courriers indésirables, ouvrez un ticket de support et demandez à l’agent de support d’envoyer vos messages en tant que faux positifs à nos analystes de courrier indésirable. Préparez-vous à fournir des exemples de messages qui incluent tous les en-têtes de message.
