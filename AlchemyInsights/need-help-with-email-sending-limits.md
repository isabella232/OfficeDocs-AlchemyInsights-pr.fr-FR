---
title: Vous avez besoin d’aide sur les limites d’envoi des e-mails ?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44328784"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="7864a-102">Vous avez besoin d’aide sur les limites d’envoi des e-mails ?</span><span class="sxs-lookup"><span data-stu-id="7864a-102">Need help with email sending limits?</span></span>

<span data-ttu-id="7864a-103">Vous trouverez ci-dessous les **limites d’envoi par la conception** appliquées dans le service.</span><span class="sxs-lookup"><span data-stu-id="7864a-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="7864a-104">Vous trouverez plus d’informations sur ces limites [ici](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="7864a-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="7864a-105">Pour décourager la livraison de messages en bloc non sollicités, nous appliquons des **limites de débit maximal pour les destinataires par utilisateur à tous les messages internes et sortants**.</span><span class="sxs-lookup"><span data-stu-id="7864a-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="7864a-106">Pour toutes les références SKU, cette limite est de **10 000 destinataires par jour**.</span><span class="sxs-lookup"><span data-stu-id="7864a-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="7864a-107">Les clients qui doivent envoyer légitimement des e-mails commerciaux en nombre (par exemple, des bulletins d’information des clients) doivent faire appel à des fournisseurs tiers spécialisés dans ces services.</span><span class="sxs-lookup"><span data-stu-id="7864a-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="7864a-108">**Remarque** : une fois la limite de débit maximale pour tous les destinataires atteinte, il est impossible d’envoyer des messages à partir de la boîte aux lettres tant que le nombre de destinataires des messages envoyés au cours des dernières 24 heures n’est pas redescendu en dessous de la limite.</span><span class="sxs-lookup"><span data-stu-id="7864a-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="7864a-109">L’utilisateur ne pourra pas envoyer de messages d’ici là.</span><span class="sxs-lookup"><span data-stu-id="7864a-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="7864a-110">La limite de débit de **30 messages par minute** est appliquée sur toutes les références SKU.</span><span class="sxs-lookup"><span data-stu-id="7864a-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="7864a-111">Cet élément détermine le nombre de messages qu'un utilisateur peut envoyer à partir de son compte Exchange Online pendant une période spécifiée.</span><span class="sxs-lookup"><span data-stu-id="7864a-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="7864a-112">Le **nombre maximal de destinataires autorisés dans les champs À, Cc et Cci** pour un seul e-mail sur toutes les références SKU est de **1000**.</span><span class="sxs-lookup"><span data-stu-id="7864a-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="7864a-113">Pour personnaliser cette limite, rendez-vous [ici](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="7864a-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
