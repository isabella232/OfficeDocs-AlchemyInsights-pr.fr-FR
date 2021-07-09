---
title: Pool de relais sortants
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339964"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="68f78-102">Pool de relais sortants</span><span class="sxs-lookup"><span data-stu-id="68f78-102">Outbound relay pool</span></span>

<span data-ttu-id="68f78-103">Microsoft modifie la configuration pour relayer ou transmettre des messages électroniques via Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68f78-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="68f78-104">Dans certains scénarios, les messages sont transmis ou relayés via Microsoft 365'aide d’un pool de relais spécial.</span><span class="sxs-lookup"><span data-stu-id="68f78-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="68f78-105">Les messages envoyés à l’aide du pool de relais peuvent se retrouver dans le dossier courrier indésirable du destinataire.</span><span class="sxs-lookup"><span data-stu-id="68f78-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="68f78-106">Pour plus d’informations, voir Pools de remise [sortants](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="68f78-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="68f78-107">Pour éviter un scénario d’utilisation du pool de relais, assurez-vous que les messages transmis/relayés répondent à l’un des critères suivants :</span><span class="sxs-lookup"><span data-stu-id="68f78-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="68f78-108">L’expéditeur sortant est un domaine accepté du client.</span><span class="sxs-lookup"><span data-stu-id="68f78-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="68f78-109">Sender Policy Framework (SPF) passe lorsque le message est envoyé Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68f78-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="68f78-110">DomainKeys Identified Mail (DKIM) sur le domaine de l’expéditeur P2 passe lorsque le message est envoyé Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68f78-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="68f78-111">Les messages qui répondent aux critères ci-dessus ne sont pas relayés via le pool de relais.</span><span class="sxs-lookup"><span data-stu-id="68f78-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="68f78-112">Si l’enregistrement MX de votre domaine pointe vers un serveur tiers ou local, utilisez un filtrage amélioré pour vous assurer que la validation SPF est correcte pour le courrier entrant et éviter d’envoyer des messages électroniques via le pool de relais.</span><span class="sxs-lookup"><span data-stu-id="68f78-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="68f78-113">**Comment savoir si nous sommes touchés par le pool de relais ?**</span><span class="sxs-lookup"><span data-stu-id="68f78-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="68f78-114">Si vos messages électroniques transmis ou relayés utilisent l’un des critères ci-dessus, les messages ne seront pas relayés via le pool de relais.</span><span class="sxs-lookup"><span data-stu-id="68f78-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="68f78-115">Toutefois, si un message est envoyé via un pool de relais, l’adresse IP du serveur sortant se trouve dans la plage 40.95.0.0/16 et le nom du serveur sortant inclut **rly** dans le nom.</span><span class="sxs-lookup"><span data-stu-id="68f78-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

