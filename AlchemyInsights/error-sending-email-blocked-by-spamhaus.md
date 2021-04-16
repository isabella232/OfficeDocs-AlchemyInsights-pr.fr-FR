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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erreur lors de l'envoi d'un e-mail : l'hôte du client est bloqué à l'aide du courrier indésirable

L'adresse IP qui a envoyé le message figure sur une liste d'adresses ip bloqués qui appartient à [Spamhouse](https://go.microsoft.com/fwlink/p/?linkid=123245). Les raisons de blocage par spam courrier indésirable incluent des comptes compromis, des ordinateurs compromis partageant une adresse IP publique et des stratégies de fournisseur de services Internet (ISP). Les correctifs possibles sont les :
  
- Pour les messages entrants bloqués dans lequel vous contrôlez le serveur de messagerie source, vous devez déterminer la cause et supprimer le blocage du site web Spamhouse.

- Pour les messages entrants bloqués dont l'adresse IP source appartient à une autre personne, le propriétaire de l'adresse doit supprimer le blocage du site web Spamhouse. Si l'adresse IP se trouve dans la liste d'adresses ip bloqués (PBL), le propriétaire peut affecter une adresse IP statique différente ou supprimer l'adresse de la liste d'adresses en question.

- Pour les messages sortants bloqués provenant de votre domaine connecté à Microsoft, vous pouvez recevoir cette erreur si les messages sont acheminés via un service tiers. Vous pouvez utiliser un outil de recherche WHOIS pour rechercher le propriétaire de l'adresse IP bloquée.
