---
title: Erreur lors de l'envoi du courrier électronique bloqué par SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402257"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d30e9-102">Erreur lors de l'envoi du message électronique: hôte client bloqué à l'aide de Spamhaus</span><span class="sxs-lookup"><span data-stu-id="d30e9-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d30e9-103">L'adresse IP qui a envoyé le message est sur une liste rouge appartenant à [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="d30e9-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="d30e9-104">Les raisons pour lesquelles le blocage par Spamhaus incluent les comptes compromis, les machines compromises partageant une adresse IP publique et les stratégies de fournisseur de services Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="d30e9-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="d30e9-105">Les corrections possibles sont les suivantes:</span><span class="sxs-lookup"><span data-stu-id="d30e9-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="d30e9-106">Pour les messages entrants bloqués vers Office 365 où vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="d30e9-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="d30e9-107">Pour les messages entrants bloqués vers Office 365 où l'adresse IP source appartient à une autre personne, le propriétaire de l'adresse doit supprimer le blocage du site Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="d30e9-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="d30e9-108">Si l'adresse IP se trouve dans la liste de blocage de stratégie (PBL), le propriétaire peut attribuer une autre adresse IP statique ou supprimer l'adresse de l'PBL.</span><span class="sxs-lookup"><span data-stu-id="d30e9-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="d30e9-109">Pour les messages sortants bloqués à partir de votre domaine Office 365, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers.</span><span class="sxs-lookup"><span data-stu-id="d30e9-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="d30e9-110">Vous pouvez utiliser un outil de recherche WHOIS pour trouver le propriétaire de l'adresse IP bloquée.</span><span class="sxs-lookup"><span data-stu-id="d30e9-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

