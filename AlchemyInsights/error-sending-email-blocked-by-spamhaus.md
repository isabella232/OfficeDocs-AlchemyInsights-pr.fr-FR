---
title: Erreur d’envoi de courrier électronique bloqué par SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288507"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f42f9-102">Erreur d’envoi de courrier électronique : hôte du Client bloquée à l’aide de Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f42f9-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f42f9-p101">L’adresse IP qui a envoyé le message est une liste de bloc détenus par [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Les raisons pour bloqué par Spamhaus les comptes compromis, les compromis machines partage une adresse IP publique et des stratégies de fournisseur de services (Internet). Solutions possibles sont les suivants :</span><span class="sxs-lookup"><span data-stu-id="f42f9-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="f42f9-106">Pour les messages entrants bloqués vers Office 365 permet de contrôler le serveur de messagerie source, vous devez déterminer la cause et supprimer le bloc depuis le site Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f42f9-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="f42f9-p102">Pour les messages entrants bloqués vers Office 365, où l’adresse IP source appartient à une autre personne, le propriétaire de l’adresse doit supprimer le bloc depuis le site Web Spamhaus. Si l’adresse IP est sur la liste de bloc de stratégie (PBL), le propriétaire peut affecter une autre adresse IP statique ou supprimer l’adresse de la PBL.</span><span class="sxs-lookup"><span data-stu-id="f42f9-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="f42f9-p103">Pour les messages sortants bloqués à partir de votre domaine à Office 365, vous pouvez recevoir cette erreur si les messages sont acheminés via un service partie 3. Vous pouvez utiliser un outil de recherche de WHOIS pour rechercher le propriétaire d’adresses IP bloqué.</span><span class="sxs-lookup"><span data-stu-id="f42f9-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

