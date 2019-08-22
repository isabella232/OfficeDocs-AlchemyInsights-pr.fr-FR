---
title: Erreur lors de l’envoi du courrier électronique bloqué par SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527130"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erreur lors de l’envoi du message électronique: hôte client bloqué à l’aide de Spamhaus

L’adresse IP qui a envoyé le message est sur une liste rouge appartenant à [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Les raisons pour lesquelles le blocage par Spamhaus incluent les comptes compromis, les machines compromises partageant une adresse IP publique et les stratégies de fournisseur de services Internet (ISP). Les corrections possibles sont les suivantes:
  
- Pour les messages entrants bloqués vers Office 365 où vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site Web Spamhaus.

- Pour les messages entrants bloqués vers Office 365 où l’adresse IP source appartient à une autre personne, le propriétaire de l’adresse doit supprimer le blocage du site Web Spamhaus. Si l’adresse IP se trouve dans la liste de blocage de stratégie (PBL), le propriétaire peut attribuer une autre adresse IP statique ou supprimer l’adresse de l’PBL.

- Pour les messages sortants bloqués à partir de votre domaine Office 365, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers. Vous pouvez utiliser un outil de recherche WHOIS pour trouver le propriétaire de l’adresse IP bloquée.
