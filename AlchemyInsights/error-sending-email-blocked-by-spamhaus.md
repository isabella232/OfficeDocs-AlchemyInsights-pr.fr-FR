---
title: Erreur lors de l'envoi de courriers électroniques bloqués par SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813722"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="4456a-102">Erreur lors de l'envoi d'un e-mail : l'hôte du client est bloqué à l'aide du courrier indésirable</span><span class="sxs-lookup"><span data-stu-id="4456a-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="4456a-103">L'adresse IP qui a envoyé le message figure sur une liste d'adresses ip bloqués qui appartient à [Spamhouse](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="4456a-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="4456a-104">Les raisons de blocage par spam courrier indésirable incluent des comptes compromis, des ordinateurs compromis partageant une adresse IP publique et des stratégies de fournisseur de services Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="4456a-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="4456a-105">Les correctifs possibles sont les :</span><span class="sxs-lookup"><span data-stu-id="4456a-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="4456a-106">Pour les messages entrants bloqués dans lequel vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site web Spamhouse.</span><span class="sxs-lookup"><span data-stu-id="4456a-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="4456a-107">Pour les messages entrants bloqués dont l'adresse IP source appartient à une autre personne, le propriétaire de l'adresse doit supprimer le blocage du site web Spamhouse.</span><span class="sxs-lookup"><span data-stu-id="4456a-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="4456a-108">Si l'adresse IP se trouve dans la liste d'adresses ip bloqués (PBL), le propriétaire peut affecter une adresse IP statique différente ou supprimer l'adresse de la liste d'adresses en question.</span><span class="sxs-lookup"><span data-stu-id="4456a-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="4456a-109">Pour les messages sortants bloqués provenant de votre domaine connecté à Microsoft, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers.</span><span class="sxs-lookup"><span data-stu-id="4456a-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="4456a-110">Vous pouvez utiliser un outil de recherche WHOIS pour rechercher le propriétaire de l'adresse IP bloquée.</span><span class="sxs-lookup"><span data-stu-id="4456a-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
