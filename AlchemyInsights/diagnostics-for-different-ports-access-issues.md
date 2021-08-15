---
title: Diagnostics pour différents problèmes d’accès aux ports
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030900"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostics pour différents problèmes d’accès aux ports

Pour résoudre les différents problèmes d’accès aux ports, effectuez les étapes suivantes :

1. Arrêtez/deallocatez la machine virtuelle (VM) à partir du portail, redémarrez la VM et testez à nouveau. 
2. Contrôlez les paramètres réseau de votre VM pour déterminer si des groupes de sécurité réseau (NSG) bloquent le trafic. Vous pouvez également utiliser [Outil de vérification du flux IP de Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) pour vérifier si les NSG bloquent le trafic, les itinéraires définis par l’utilisateur qui achemine votre trafic vers l’itinéraire local (« Chemin par défaut » 0.0.0.0/0) ou vers un équipement réseau.
Si vous rencontrez toujours des problèmes après avoir essayé les étapes ci-dessus, veuillez fournir le nom de la VM et le port TCP sur lequel vous essayez d'envoyer du courrier pour un diagnostic plus approfondi.

**Documents recommandés**

[Limitations et recommandations pour l’envoi de messages sortants sur le port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)