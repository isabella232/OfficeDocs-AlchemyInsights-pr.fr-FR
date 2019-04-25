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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erreur lors de l'envoi du message électronique: hôte client bloqué à l'aide de Spamhaus

L'adresse IP qui a envoyé le message est sur une liste rouge appartenant à [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Les raisons pour lesquelles le blocage par Spamhaus incluent les comptes compromis, les machines compromises partageant une adresse IP publique et les stratégies de fournisseur de services Internet (ISP). Les corrections possibles sont les suivantes:
  
- Pour les messages entrants bloqués vers Office 365 où vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site Web Spamhaus.
    
- Pour les messages entrants bloqués vers Office 365 où l'adresse IP source appartient à une autre personne, le propriétaire de l'adresse doit supprimer le blocage du site Web Spamhaus. Si l'adresse IP se trouve dans la liste de blocage de stratégie (PBL), le propriétaire peut attribuer une autre adresse IP statique ou supprimer l'adresse de l'PBL.
    
- Pour les messages sortants bloqués à partir de votre domaine Office 365, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers. Vous pouvez utiliser un outil de recherche WHOIS pour trouver le propriétaire de l'adresse IP bloquée.
    

