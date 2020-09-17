---
title: Erreur lors de l’envoi du courrier électronique bloqué par SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783801"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="12380-102">Erreur lors de l’envoi du message électronique : hôte client bloqué à l’aide de Spamhaus</span><span class="sxs-lookup"><span data-stu-id="12380-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="12380-103">L’adresse IP qui a envoyé le message est sur une liste rouge appartenant à [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="12380-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="12380-104">Les raisons pour lesquelles le blocage par Spamhaus incluent les comptes compromis, les machines compromises partageant une adresse IP publique et les stratégies de fournisseur de services Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="12380-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="12380-105">Les corrections possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="12380-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="12380-106">Pour les messages entrants bloqués lorsque vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="12380-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="12380-107">Pour les messages entrants bloqués lorsque l’adresse IP source appartient à une autre personne, le propriétaire de l’adresse doit supprimer le blocage du site Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="12380-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="12380-108">Si l’adresse IP se trouve dans la liste de blocage de stratégie (PBL), le propriétaire peut attribuer une autre adresse IP statique ou supprimer l’adresse de l’PBL.</span><span class="sxs-lookup"><span data-stu-id="12380-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="12380-109">Pour les messages sortants bloqués provenant de votre domaine connecté à Microsoft, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers.</span><span class="sxs-lookup"><span data-stu-id="12380-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="12380-110">Vous pouvez utiliser un outil de recherche WHOIS pour trouver le propriétaire de l’adresse IP bloquée.</span><span class="sxs-lookup"><span data-stu-id="12380-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
