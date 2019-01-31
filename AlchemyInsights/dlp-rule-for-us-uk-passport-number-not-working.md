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
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656421"
---
Vous rencontrez des problèmes avec **Data Loss Prevention (DLP)** ne fonctionne ne pas pour le contenu contenant un **US / numéro de passeport (Royaume-Uni)** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Dans ce cas, assurez-vous que votre contenu contient les informations nécessaires pour que la stratégie DLP est recherchez lorsqu’elle est évaluée. 
  
Par exemple, pour un **US / numéro de passeport Royaume-Uni** stratégie configurée avec un niveau de confiance de 75 %, ce qui suit sont évalué et doivent être détecté pour déclencher la règle 
  
- **[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neuf chiffres 
    
- **[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neuf chiffres consécutifs 
    
- **[Somme de contrôle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’existe aucune somme de contrôle 
    
- **[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Une stratégie DLP est convaincu que ce type d’informations sensibles a été détecté à 75 % if, au sein d’une proximité de 300 caractères : 
    
  - La fonction Func_usa_uk_passport trouve un contenu qui correspond au modèle.
    
  - Un mot clé figurant dans la liste Keyword_passport est trouvé.
    
    Par exemple, l’exemple suivant déclenche pour les **US / numéro de passeport Royaume-Uni** stratégie : numéro de passeport 123456789 
    
Pour plus d’informations sur ce qui est requis pour un US / numéro de passeport Royaume-Uni soient détectées pour votre contenu, consultez la section suivante de cet article : [apparence que le sensibles Types d’informations pour les États-Unis / numéro de passeport (Royaume-Uni)](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
À l’aide d’un type de différentes informations sensibles intégrés, consultez l’article suivant pour plus d’informations sur ce qui est nécessaire pour les autres types : [recherchez ce que le sensibles Types d’informations](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

