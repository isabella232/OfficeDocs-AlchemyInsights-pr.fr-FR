---
title: Utilisation de DLP dans les règles de transport
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827214"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="156d4-102">Utilisation de DLP dans les règles de transport</span><span class="sxs-lookup"><span data-stu-id="156d4-102">Using DLP in transport rules</span></span>

<span data-ttu-id="156d4-103">Pour intégrer la protection contre la perte de données (DLP) dans un transport existant, utilisez la condition « **si le message contient... Informations sensibles** » dans le paramètre de règle de transport.</span><span class="sxs-lookup"><span data-stu-id="156d4-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="156d4-104">**Pour plus d’informations, consultez la rubrique :**.</span><span class="sxs-lookup"><span data-stu-id="156d4-104">**For more details, see:**</span></span>

- <span data-ttu-id="156d4-105">Types d’informations sensibles DLP intégrés dans les règles de transport : [Intégrer des règles d’informations sensibles](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="156d4-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="156d4-106">Vous pouvez également tester la règle avec ou sans test de stratégie à l’aide du mode test sur la règle.</span><span class="sxs-lookup"><span data-stu-id="156d4-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="156d4-107">Vous devez patienter 30 minutes après la création de la règle avant de la tester.</span><span class="sxs-lookup"><span data-stu-id="156d4-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="156d4-108">Voir [Tester les règles de flux/transport de courrier](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="156d4-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="156d4-109">**Remarque** : si vous essayez d’implémenter une nouvelle stratégie DLP avec des règles de transport dans le centre d’administration Exchange, utilisez à la place les [Stratégies DLP dans le centre de sécurité et conformité](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="156d4-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
