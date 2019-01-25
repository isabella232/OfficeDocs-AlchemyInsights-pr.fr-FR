---
title: Règles DLP pour US / numéro de passeport Royaume-Uni ne fonctionne ne pas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468894"
---
<span data-ttu-id="e4da3-p101">Vous rencontrez des problèmes avec **Data Loss Prevention (DLP)** ne fonctionne ne pas pour le contenu contenant un **US / numéro de passeport (Royaume-Uni)** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Dans ce cas, assurez-vous que votre contenu contient les informations nécessaires pour que la stratégie DLP est recherchez lorsqu’elle est évaluée.</span><span class="sxs-lookup"><span data-stu-id="e4da3-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="e4da3-104">Par exemple, pour un **US / numéro de passeport Royaume-Uni** stratégie configurée avec un niveau de confiance de 75 %, ce qui suit sont évalué et doivent être détecté pour déclencher la règle</span><span class="sxs-lookup"><span data-stu-id="e4da3-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="e4da3-105">**[Format :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neuf chiffres</span><span class="sxs-lookup"><span data-stu-id="e4da3-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="e4da3-106">**[Modèle :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neuf chiffres consécutifs</span><span class="sxs-lookup"><span data-stu-id="e4da3-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="e4da3-107">**[Somme de contrôle :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’existe aucune somme de contrôle</span><span class="sxs-lookup"><span data-stu-id="e4da3-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="e4da3-108">**[Définition :](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Une stratégie DLP est convaincu que ce type d’informations sensibles a été détecté à 75 % if, au sein d’une proximité de 300 caractères :</span><span class="sxs-lookup"><span data-stu-id="e4da3-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e4da3-109">La fonction Func_usa_uk_passport trouve un contenu qui correspond au modèle.</span><span class="sxs-lookup"><span data-stu-id="e4da3-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="e4da3-110">Un mot clé figurant dans la liste Keyword_passport est trouvé.</span><span class="sxs-lookup"><span data-stu-id="e4da3-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="e4da3-111">Par exemple, l’exemple suivant déclenche pour les **US / numéro de passeport Royaume-Uni** stratégie : numéro de passeport 123456789</span><span class="sxs-lookup"><span data-stu-id="e4da3-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="e4da3-112">Pour plus d’informations sur ce qui est requis pour un US / numéro de passeport Royaume-Uni soient détectées pour votre contenu, consultez la section suivante de cet article : [apparence que le sensibles Types d’informations pour les États-Unis / numéro de passeport (Royaume-Uni)](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="e4da3-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="e4da3-113">À l’aide d’un type de différentes informations sensibles intégrés, consultez l’article suivant pour plus d’informations sur ce qui est nécessaire pour les autres types : [recherchez ce que le sensibles Types d’informations](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e4da3-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

