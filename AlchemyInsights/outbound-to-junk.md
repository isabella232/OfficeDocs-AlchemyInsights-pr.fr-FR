---
title: Courrier électronique sortant vers le dossier courrier indésirable
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769181"
---
# <a name="outbound-email-to-junk-email-folder"></a>Courrier électronique sortant vers le dossier courrier indésirable

Si vous constatez que les messages sortants sont marqués comme courrier indésirable, procédez comme suit :

- Si vous ne l’avez pas encore fait, envisagez de [configurer les notifications de stratégie de courrier indésirable sortant](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Utilisez le [suivi des messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) pour voir si le message sortant a la valeur de l’événement **courrier indésirable** avec les détails supplémentaires : **utiliser un pool de remise à risque élevé**.

  Pour ces messages, vérifiez le contenu du message pour voir ce qui peut être considéré comme du courrier indésirable. Par exemple, les signatures peuvent parfois causer des problèmes à de nombreux utilisateurs.

  Si vous avez plusieurs exemples de messages sortants légitimes marqués comme courriers indésirables, ouvrez un ticket de support et demandez à l’agent de support d’envoyer vos messages en tant que faux positifs à nos analystes de courrier indésirable. Préparez-vous à fournir des exemples de messages qui incluent tous les en-têtes de message.
