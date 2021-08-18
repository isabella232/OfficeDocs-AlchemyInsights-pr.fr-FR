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
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326075"
---
# <a name="outbound-relay-pool"></a>Pool de relais sortants

Microsoft modifie la configuration pour relayer ou transmettre des messages électroniques via Microsoft 365. Dans certains scénarios, les messages sont transmis ou relayés via Microsoft 365'aide d’un pool de relais spécial. Les messages envoyés à l’aide du pool de relais peuvent se retrouver dans le dossier courrier indésirable du destinataire. Pour plus d’informations, voir Pools de remise [sortants](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Pour éviter un scénario d’utilisation du pool de relais, assurez-vous que les messages transmis/relayés répondent à l’un des critères suivants :

- L’expéditeur sortant est un domaine accepté du client.
- Sender Policy Framework (SPF) passe lorsque le message est envoyé Microsoft 365.
- DomainKeys Identified Mail (DKIM) sur le domaine de l’expéditeur P2 passe lorsque le message est envoyé Microsoft 365.
 
Les messages qui répondent aux critères ci-dessus ne sont pas relayés via le pool de relais.

Si l’enregistrement MX de votre domaine pointe vers un serveur tiers ou local, utilisez un filtrage amélioré pour vous assurer que la validation SPF est correcte pour le courrier entrant et éviter d’envoyer des messages électroniques via le pool de relais.

**Comment savoir si nous sommes touchés par le pool de relais ?**

Si vos messages électroniques transmis ou relayés utilisent l’un des critères ci-dessus, les messages ne seront pas relayés via le pool de relais. Toutefois, si un message est envoyé via un pool de relais, l’adresse IP du serveur sortant se trouve dans la plage 40.95.0.0/16 et le nom du serveur sortant inclut **rly** dans le nom.

