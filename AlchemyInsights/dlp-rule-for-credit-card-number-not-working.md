---
title: La règle DLP pour le numéro de carte de crédit ne fonctionne pas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529953"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="87874-102">Problèmes liés à DLP avec les numéros de carte de crédit</span><span class="sxs-lookup"><span data-stu-id="87874-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="87874-103">Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de carte bancaire** lors de l’utilisation d’un type d’informations sensibles DLP dans O365?</span><span class="sxs-lookup"><span data-stu-id="87874-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="87874-104">Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour déclencher la stratégie DLP lors de son évaluation.</span><span class="sxs-lookup"><span data-stu-id="87874-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="87874-105">Par exemple, pour une **stratégie de carte de crédit** configurée avec un niveau de confiance de 85%, les éléments suivants sont évalués et doivent être détectés pour le déclenchement de la règle:</span><span class="sxs-lookup"><span data-stu-id="87874-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="87874-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chiffres qui peuvent être mis en forme ou non (dddddddddddddddd) et doivent réussir le test Luhn.</span><span class="sxs-lookup"><span data-stu-id="87874-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="87874-107">**[Modèle:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modèle très complexe et robuste qui détecte les cartes de toutes les principales marques dans le monde, notamment les cartes Visa, MasterCard, Discover Card, JCB, American Express, les cartes cadeaux et les cartes dîner.</span><span class="sxs-lookup"><span data-stu-id="87874-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="87874-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Oui, la somme de contrôle Luhn</span><span class="sxs-lookup"><span data-stu-id="87874-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="87874-109">**[Définition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Une stratégie DLP est sûre à 85% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères:</span><span class="sxs-lookup"><span data-stu-id="87874-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="87874-110">La fonction Func_credit_card trouve un contenu qui correspond au modèle.</span><span class="sxs-lookup"><span data-stu-id="87874-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="87874-111">L’une des affirmations suivantes est vraie :</span><span class="sxs-lookup"><span data-stu-id="87874-111">One of the following is true:</span></span>

  - <span data-ttu-id="87874-112">Un mot clé figurant dans la liste Keyword_cc_verification est trouvé.</span><span class="sxs-lookup"><span data-stu-id="87874-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="87874-113">Un mot clé depuis Keyword_cc_name est trouvé.</span><span class="sxs-lookup"><span data-stu-id="87874-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="87874-114">La fonction Func_expiration_date trouve une date au format correct.</span><span class="sxs-lookup"><span data-stu-id="87874-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="87874-115">Le checksum passe</span><span class="sxs-lookup"><span data-stu-id="87874-115">The checksum passes</span></span>

    <span data-ttu-id="87874-116">Par exemple, l’exemple suivant se déclenche pour une stratégie de numéro de carte de crédit DLP:</span><span class="sxs-lookup"><span data-stu-id="87874-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="87874-117">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="87874-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="87874-118">Date d’expiration: 2/2009</span><span class="sxs-lookup"><span data-stu-id="87874-118">Expires: 2/2009</span></span>

<span data-ttu-id="87874-119">Pour plus d’informations sur les éléments requis pour la détection d’un **numéro de carte de crédit** pour votre contenu, reportez-vous à la section suivante de cet article: [ce que recherche les types d’informations sensibles pour la carte de crédit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="87874-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="87874-120">À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types: [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="87874-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  