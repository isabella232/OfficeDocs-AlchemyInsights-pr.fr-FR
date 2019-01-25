---
title: Règles DLP pour le numéro de carte de crédit ne fonctionne ne pas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469327"
---
<span data-ttu-id="9cf64-p101">Vous rencontrez des problèmes avec **Data Loss Prevention (DLP)** ne fonctionne ne pas pour le contenu contenant un **Numéro de carte de crédit** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Dans ce cas, assurez-vous que votre contenu contient les informations nécessaires pour déclencher le la stratégie DLP lorsqu’elle est évaluée. Par exemple, pour une **carte de crédit stratégie** configurée avec un niveau de confiance de 85 %, les éléments suivants sont évaluées et doivent être détectées pour déclencher la règle :</span><span class="sxs-lookup"><span data-stu-id="9cf64-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="9cf64-105">**[Format :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chiffres qui peuvent être mis en forme ou non mis en forme (dddddddddddddddd) et doit réussir le test Luhn.</span><span class="sxs-lookup"><span data-stu-id="9cf64-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="9cf64-106">**[Modèle :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modèle robuste et très complexe qui détecte les cartes de visite à partir de toutes les marques principales dans le monde, y compris Visa Mastercard, carte Discover, JCB, American Express, cartes cadeaux et cartes dîner.</span><span class="sxs-lookup"><span data-stu-id="9cf64-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="9cf64-107">**[Somme de contrôle :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Oui, la somme de contrôle Luhn</span><span class="sxs-lookup"><span data-stu-id="9cf64-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="9cf64-108">**[Définition :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Une stratégie DLP est de 85 % convaincu que ce type d’informations sensibles a été détecté if, au sein d’une proximité de 300 caractères :</span><span class="sxs-lookup"><span data-stu-id="9cf64-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="9cf64-109">La fonction Func_credit_card trouve un contenu qui correspond au modèle.</span><span class="sxs-lookup"><span data-stu-id="9cf64-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="9cf64-110">L’une des affirmations suivantes est vraie :</span><span class="sxs-lookup"><span data-stu-id="9cf64-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="9cf64-111">Un mot clé figurant dans la liste Keyword_cc_verification est trouvé.</span><span class="sxs-lookup"><span data-stu-id="9cf64-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="9cf64-112">Un mot clé figurant dans la liste Keyword_cc_name est trouvé.</span><span class="sxs-lookup"><span data-stu-id="9cf64-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="9cf64-113">La fonction Func_expiration_date trouve une date au format correct.</span><span class="sxs-lookup"><span data-stu-id="9cf64-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="9cf64-114">La somme de contrôle est correcte.</span><span class="sxs-lookup"><span data-stu-id="9cf64-114">The checksum passes</span></span>
    
    <span data-ttu-id="9cf64-115">Par exemple, l’exemple suivant déclenche pour une stratégie de numéro de carte de crédit DLP :</span><span class="sxs-lookup"><span data-stu-id="9cf64-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="9cf64-116">Visa : 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="9cf64-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="9cf64-117">Date d’expiration : 2/2009</span><span class="sxs-lookup"><span data-stu-id="9cf64-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="9cf64-118">Pour plus d’informations sur ce qui est requis pour un **Numéro de carte de crédit** à être détectées pour votre contenu, voir la section suivante de cet article : [Ce que le sensibles Types d’informations recherchez ce numéro de carte de crédit](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="9cf64-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="9cf64-119">À l’aide d’un type de différentes informations sensibles intégrés, consultez l’article suivant pour plus d’informations sur ce qui est nécessaire pour les autres types : [recherchez ce que le sensibles Types d’informations](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="9cf64-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

