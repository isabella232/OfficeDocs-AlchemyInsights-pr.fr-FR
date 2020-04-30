---
title: Utilisation de DLP dans les règles de transport
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915095"
---
# <a name="using-dlp-in-transport-rules"></a>Utilisation de DLP dans les règles de transport

Pour intégrer la protection contre la perte de données (DLP) dans un transport existant, utilisez la condition « **si le message contient... Informations sensibles** » dans le paramètre de règle de transport.

**Pour plus d’informations, consultez la rubrique :**.

- Types d’informations sensibles DLP intégrés dans les règles de transport : [Intégrer des règles d’informations sensibles](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Vous pouvez également tester la règle avec ou sans test de stratégie à l’aide du mode test sur la règle.  Vous devez patienter 30 minutes après la création de la règle avant de la tester.

- Voir [Tester les règles de flux/transport de courrier](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Remarque** : si vous essayez d’implémenter une nouvelle stratégie DLP avec des règles de transport dans le centre d’administration Exchange, utilisez à la place les [Stratégies DLP dans le centre de sécurité et conformité](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
