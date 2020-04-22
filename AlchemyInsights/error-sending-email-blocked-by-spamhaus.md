---
title: Erreur lors de l’envoi du courrier électronique bloqué par SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714256"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erreur lors de l’envoi du message électronique : hôte client bloqué à l’aide de Spamhaus

L’adresse IP qui a envoyé le message est sur une liste rouge appartenant à [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Les raisons pour lesquelles le blocage par Spamhaus incluent les comptes compromis, les machines compromises partageant une adresse IP publique et les stratégies de fournisseur de services Internet (ISP). Les corrections possibles sont les suivantes :
  
- Pour les messages entrants bloqués lorsque vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site Web Spamhaus.

- Pour les messages entrants bloqués lorsque l’adresse IP source appartient à une autre personne, le propriétaire de l’adresse doit supprimer le blocage du site Web Spamhaus. Si l’adresse IP se trouve dans la liste de blocage de stratégie (PBL), le propriétaire peut attribuer une autre adresse IP statique ou supprimer l’adresse de l’PBL.

- Pour les messages sortants bloqués provenant de votre domaine connecté à Microsoft, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers. Vous pouvez utiliser un outil de recherche WHOIS pour trouver le propriétaire de l’adresse IP bloquée.
