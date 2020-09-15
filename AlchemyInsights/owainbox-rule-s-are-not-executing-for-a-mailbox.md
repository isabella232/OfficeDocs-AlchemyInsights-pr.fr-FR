---
title: 1332 la ou les règles de boîte de réception OWA ne s’exécutent pas pour une boîte aux lettres
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
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721589"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="e7959-102">Une règle de boîte de réception ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="e7959-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="e7959-103">Vérifiez les paramètres suivants dans Outlook sur le Web :</span><span class="sxs-lookup"><span data-stu-id="e7959-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="e7959-104">Un message peut être redirigé, transféré ou une réponse est automatiquement basée sur les règles de boîte de réception une seule fois.</span><span class="sxs-lookup"><span data-stu-id="e7959-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="e7959-105">Une règle de redirection (une règle de boîte de réception ou une règle de flux de messagerie, également appelée règle de transport) peut ajouter un maximum de dix destinataires de transfert à un message.</span><span class="sxs-lookup"><span data-stu-id="e7959-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="e7959-106">Pour plus d’informations, consultez les [limitations de journal, de transport et de règles de boîte de réception](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="e7959-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="e7959-107">Les règles de boîte de réception ne fonctionnent pas sur l’autre boîte aux lettres de journalisation.</span><span class="sxs-lookup"><span data-stu-id="e7959-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="e7959-108">Pour plus d’informations sur l’autre boîte aux lettres de journalisation, voir [autre boîte aux lettres de journalisation](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e7959-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="e7959-109">Pour résoudre ces problèmes, reportez-vous à la rubrique [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="e7959-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="e7959-110">Si les problèmes précédents ne s’appliquent pas, exécutez le rapport de diagnostic des règles de boîte de réception avant de remonter le problème vers le support Microsoft :</span><span class="sxs-lookup"><span data-stu-id="e7959-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="e7959-111">Ouvrez la boîte aux lettres dans Outlook sur le Web, puis cliquez sur</span><span class="sxs-lookup"><span data-stu-id="e7959-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="e7959-112">**Paramètres**  >  **Afficher tous les paramètres Outlook**  >  **Courrier électronique**  >  **Règles**.</span><span class="sxs-lookup"><span data-stu-id="e7959-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="e7959-113">Au bas de la page, cliquez sur **si vos règles ne fonctionnent pas cliquez ici pour générer un rapport de diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="e7959-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
