---
title: La règle DLP pour le numéro de passeport US/UK ne fonctionne pas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404379"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="a8945-102">Problèmes liés aux numéros de passeport DLP-US/UK</span><span class="sxs-lookup"><span data-stu-id="a8945-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="a8945-103">Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de passeport US/UK** lorsque vous utilisez un type d'informations sensibles DLP dans O365?</span><span class="sxs-lookup"><span data-stu-id="a8945-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a8945-104">Si c'est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lors de l'évaluation.</span><span class="sxs-lookup"><span data-stu-id="a8945-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="a8945-105">Par exemple, pour une stratégie de **numéro de passeport US/UK** configurée avec un niveau de confiance de 75%, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche</span><span class="sxs-lookup"><span data-stu-id="a8945-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="a8945-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neuf chiffres</span><span class="sxs-lookup"><span data-stu-id="a8945-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="a8945-107">**[Modèle:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neuf chiffres consécutifs</span><span class="sxs-lookup"><span data-stu-id="a8945-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="a8945-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n'y a pas de checksum</span><span class="sxs-lookup"><span data-stu-id="a8945-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="a8945-109">**[Définition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Une stratégie DLP est sûre à 75% d'avoir détecté ce type d'informations sensibles si, dans une proximité de 300 caractères:</span><span class="sxs-lookup"><span data-stu-id="a8945-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a8945-110">La fonction Func_usa_uk_passport trouve un contenu qui correspond au modèle.</span><span class="sxs-lookup"><span data-stu-id="a8945-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="a8945-111">Un mot clé figurant dans la liste Keyword_passport est trouvé.</span><span class="sxs-lookup"><span data-stu-id="a8945-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="a8945-112">Par exemple, l'exemple suivant se déclenche pour la stratégie de **numéro de passeport US/UK** : numéro de passeport américain 123456789</span><span class="sxs-lookup"><span data-stu-id="a8945-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="a8945-113">Pour plus d'informations sur les éléments requis pour la détection d'un numéro de passeport US/UK pour votre contenu, consultez la section suivante de cet article: [ce que les types d'informations sensibles recherchent sur le numéro de passeport US/UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="a8945-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="a8945-114">À l'aide d'un type d'informations sensibles intégré différent, consultez l'article suivant pour obtenir des informations sur les éléments requis pour les autres types: [ce que recherche les types d'informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a8945-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

