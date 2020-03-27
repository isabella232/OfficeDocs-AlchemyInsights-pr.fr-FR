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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977196"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d3c4c-102">Problèmes liés à DLP avec les numéros de carte de crédit</span><span class="sxs-lookup"><span data-stu-id="d3c4c-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d3c4c-103">**Important**: pendant ces temps inégalés, nous faisons en sorte de s’assurer que les services SharePoint Online et OneDrive restent hautement disponibles : consultez les [ajustements de fonctionnalité temporaire SharePoint Online](https://aka.ms/ODSPAdjustments) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d3c4c-104">**Problèmes liés à DLP avec les numéros de carte de crédit**</span><span class="sxs-lookup"><span data-stu-id="d3c4c-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d3c4c-105">Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de carte bancaire** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ?</span><span class="sxs-lookup"><span data-stu-id="d3c4c-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d3c4c-106">Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour déclencher la stratégie DLP lors de son évaluation.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d3c4c-107">Par exemple, pour une **stratégie de carte de crédit** configurée avec un niveau de confiance de 85%, les éléments suivants sont évalués et doivent être détectés pour le déclenchement de la règle :</span><span class="sxs-lookup"><span data-stu-id="d3c4c-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d3c4c-108">**[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chiffres qui peuvent être mis en forme ou non (dddddddddddddddd) et doivent réussir le test Luhn.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d3c4c-109">**[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modèle très complexe et robuste qui détecte les cartes de toutes les principales marques dans le monde, notamment les cartes Visa, MasterCard, Discover Card, JCB, American Express, les cartes cadeaux et les cartes dîner.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d3c4c-110">**[Checksum :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Oui, la somme de contrôle Luhn</span><span class="sxs-lookup"><span data-stu-id="d3c4c-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d3c4c-111">**[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Une stratégie DLP est sûre à 85% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :</span><span class="sxs-lookup"><span data-stu-id="d3c4c-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d3c4c-112">La fonction Func_credit_card trouve un contenu qui correspond au modèle.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d3c4c-113">L’une des affirmations suivantes est vraie :</span><span class="sxs-lookup"><span data-stu-id="d3c4c-113">One of the following is true:</span></span>

  - <span data-ttu-id="d3c4c-114">Un mot clé figurant dans la liste Keyword_cc_verification est trouvé.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d3c4c-115">Un mot clé depuis Keyword_cc_name est trouvé.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d3c4c-116">La fonction Func_expiration_date trouve une date au format correct.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d3c4c-117">Le checksum passe</span><span class="sxs-lookup"><span data-stu-id="d3c4c-117">The checksum passes</span></span>

    <span data-ttu-id="d3c4c-118">Par exemple, l’exemple suivant se déclenche pour une stratégie de numéro de carte de crédit DLP :</span><span class="sxs-lookup"><span data-stu-id="d3c4c-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d3c4c-119">Visa : 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d3c4c-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d3c4c-120">Date d’expiration : 2/2009</span><span class="sxs-lookup"><span data-stu-id="d3c4c-120">Expires: 2/2009</span></span>

<span data-ttu-id="d3c4c-121">Pour plus d’informations sur les éléments requis pour la détection d’un **numéro de carte de crédit** pour votre contenu, reportez-vous à la section suivante de cet article : [ce que recherche les types d’informations sensibles pour la carte de crédit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="d3c4c-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="d3c4c-122">À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d3c4c-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  