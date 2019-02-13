---
title: Erreur d’envoi de courrier électronique bloqué par SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912346"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erreur d’envoi de courrier électronique : hôte du Client bloquée à l’aide de Spamhaus

L’adresse IP qui a envoyé le message est une liste de bloc détenus par [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Les raisons pour bloqué par Spamhaus les comptes compromis, les compromis machines partage une adresse IP publique et des stratégies de fournisseur de services (Internet). Solutions possibles sont les suivants :
  
- Pour les messages entrants bloqués vers Office 365 permet de contrôler le serveur de messagerie source, vous devez déterminer la cause et supprimer le bloc depuis le site Web Spamhaus.
    
- Pour les messages entrants bloqués vers Office 365, où l’adresse IP source appartient à une autre personne, le propriétaire de l’adresse doit supprimer le bloc depuis le site Web Spamhaus. Si l’adresse IP est sur la liste de bloc de stratégie (PBL), le propriétaire peut affecter une autre adresse IP statique ou supprimer l’adresse de la PBL.
    
- Pour les messages sortants bloqués à partir de votre domaine à Office 365, vous pouvez recevoir cette erreur si les messages sont acheminés via un service partie 3. Vous pouvez utiliser un outil de recherche de WHOIS pour rechercher le propriétaire d’adresses IP bloqué.
    

