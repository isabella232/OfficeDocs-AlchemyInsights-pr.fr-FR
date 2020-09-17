---
title: Utilisation de DLP dans les règles de transport
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773161"
---
# <a name="using-dlp-in-transport-rules"></a>Utilisation de DLP dans les règles de transport

Pour intégrer la protection contre la perte de données (DLP) dans un transport existant, utilisez la condition « **si le message contient... Informations sensibles** » dans le paramètre de règle de transport.

**Pour plus d’informations, consultez la rubrique :**.

- Types d’informations sensibles DLP intégrés dans les règles de transport : [Intégrer des règles d’informations sensibles](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Vous pouvez également tester la règle avec ou sans test de stratégie à l’aide du mode test sur la règle.  Vous devez patienter 30 minutes après la création de la règle avant de la tester.

- Voir [Tester les règles de flux/transport de courrier](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Remarque** : si vous essayez d’implémenter une nouvelle stratégie DLP avec des règles de transport dans le centre d’administration Exchange, utilisez à la place les [Stratégies DLP dans le centre de sécurité et conformité](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
