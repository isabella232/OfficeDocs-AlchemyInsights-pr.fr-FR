---
title: Courrier électronique sortant vers le dossier Courrier indésirable
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
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096656"
---
# <a name="outbound-email-to-junk-email-folder"></a>Courrier électronique sortant vers le dossier Courrier indésirable

Si vous voyez des messages sortants marqués comme courrier indésirable, faites les étapes suivantes :

- Si ce n’est pas déjà fait, envisagez de [configurer des notifications de](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)stratégie de courrier indésirable sortant.

- Utilisez [le suivi des messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) pour voir si le message sortant a la valeur d’événement **Courrier** indésirable avec les détails supplémentaires : Utiliser le pool de remise à **risque élevé**.

  Pour ces messages, vérifiez le contenu du message pour voir ce qui peut être considéré comme du courrier indésirable. Par exemple, les signatures peuvent parfois provoquer des problèmes pour de nombreux utilisateurs.

  Si vous avez plusieurs exemples de messages sortants légitimes marqués comme courrier indésirable, ouvrez un ticket de support et demandez à l’agent de support de soumettre vos messages comme faux positifs à nos analystes de courrier indésirable. Soyez prêt à fournir des exemples de messages qui incluent tous les en-têtes de message.
