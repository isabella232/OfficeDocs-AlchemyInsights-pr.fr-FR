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
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511722"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="2c388-102">Courrier électronique sortant vers le dossier courrier indésirable</span><span class="sxs-lookup"><span data-stu-id="2c388-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="2c388-103">Si vous constatez que les messages sortants sont marqués comme courrier indésirable, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="2c388-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="2c388-104">Si vous ne l’avez pas encore fait, envisagez de [configurer les notifications de stratégie de courrier indésirable sortant](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="2c388-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="2c388-105">Utilisez le [suivi des messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) pour voir si le message sortant a la valeur de l’événement **courrier indésirable** avec les détails supplémentaires : **utiliser un pool de remise à risque élevé**.</span><span class="sxs-lookup"><span data-stu-id="2c388-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="2c388-106">Pour ces messages, vérifiez le contenu du message pour voir ce qui peut être considéré comme du courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="2c388-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="2c388-107">Par exemple, les signatures peuvent parfois causer des problèmes à de nombreux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="2c388-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="2c388-108">Si vous avez plusieurs exemples de messages sortants légitimes marqués comme courriers indésirables, ouvrez un ticket de support et demandez à l’agent de support d’envoyer vos messages en tant que faux positifs à nos analystes de courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="2c388-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="2c388-109">Préparez-vous à fournir des exemples de messages qui incluent tous les en-têtes de message.</span><span class="sxs-lookup"><span data-stu-id="2c388-109">Be prepared to provide sample messages that include all message headers.</span></span>
