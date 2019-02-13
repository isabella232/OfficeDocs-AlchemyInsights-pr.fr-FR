---
title: Règles DLP pour le numéro de carte de crédit ne fonctionne ne pas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919078"
---
Vous rencontrez des problèmes avec **Data Loss Prevention (DLP)** ne fonctionne ne pas pour le contenu contenant un **Numéro de carte de crédit** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Dans ce cas, assurez-vous que votre contenu contient les informations nécessaires pour déclencher le la stratégie DLP lorsqu’elle est évaluée. Par exemple, pour une **carte de crédit stratégie** configurée avec un niveau de confiance de 85 %, les éléments suivants sont évaluées et doivent être détectées pour déclencher la règle : 
  
- **[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chiffres qui peuvent être mis en forme ou non mis en forme (dddddddddddddddd) et doit réussir le test Luhn. 
    
- **[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modèle robuste et très complexe qui détecte les cartes de visite à partir de toutes les marques principales dans le monde, y compris Visa Mastercard, carte Discover, JCB, American Express, cartes cadeaux et cartes dîner. 
    
- **[Somme de contrôle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Oui, la somme de contrôle Luhn 
    
- **[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Une stratégie DLP est de 85 % convaincu que ce type d’informations sensibles a été détecté if, au sein d’une proximité de 300 caractères : 
    
  - La fonction Func_credit_card trouve un contenu qui correspond au modèle.
    
  - L’une des affirmations suivantes est vraie : 
    
  - Un mot clé figurant dans la liste Keyword_cc_verification est trouvé.
    
  - Un mot clé à partir de Keyword_cc_name est trouvé.
    
  - La fonction Func_expiration_date trouve une date au format correct.
    
  - Transmet la somme de contrôle
    
    Par exemple, l’exemple suivant déclenche pour une stratégie de numéro de carte de crédit DLP :
    
  - Visa : 4485 3647 3952 7352 
    
  - Date d’expiration : 2/2009
    
Pour plus d’informations sur ce qui est requis pour un **Numéro de carte de crédit** à être détectées pour votre contenu, voir la section suivante de cet article : [Ce que le sensibles Types d’informations recherchez ce numéro de carte de crédit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
À l’aide d’un type de différentes informations sensibles intégrés, consultez l’article suivant pour plus d’informations sur ce qui est nécessaire pour les autres types : [recherchez ce que le sensibles Types d’informations](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

