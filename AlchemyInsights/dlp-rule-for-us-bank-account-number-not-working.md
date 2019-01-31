---
title: Règles DLP pour nous numéro de compte bancaire ne fonctionne ne pas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9fd5d4736c5209f85e235dc6a0846f65f1b5f624
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656997"
---
Vous rencontrez des problèmes avec **Data Loss Prevention (DLP)** ne fonctionne ne pas pour le contenu contenant un **Numéro de compte bancaire US** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Dans ce cas, assurez-vous que votre contenu contient les informations nécessaires pour que la stratégie DLP est recherchez lorsqu’elle est évaluée. 
  
Par exemple, pour une stratégie de **Numéro de compte bancaire US** configurée avec un niveau de confiance de 85 %, les éléments suivants sont évaluées et doivent être détectées pour déclencher la règle : 
  
- **[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 chiffres 
    
- **[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** chiffres consécutifs 8-17. 
    
- **[Somme de contrôle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’existe aucune somme de contrôle 
    
- **[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Une stratégie DLP est convaincu que ce type d’informations sensibles a été détecté à 75 % if, au sein d’une proximité de 300 caractères : 
    
  - L’expression régulière Regex_usa_bank_account_number recherche de contenu qui correspond au modèle
    
  - Un mot clé figurant dans la liste Keyword_usa_Bank_Account est trouvé.
    
    Par exemple, l’exemple suivant déclenche pour la stratégie de **Numéro de compte bancaire US** : 78344011 compte courant 
    
Pour plus d’informations sur ce qui est requis pour un **Numéro de compte bancaire US** à être détectées pour votre contenu, voir la section suivante de cet article : [Ce que le sensibles Types d’informations rechercher le numéro de compte bancaire US](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
À l’aide d’un type de différentes informations sensibles intégrés, consultez l’article suivant pour plus d’informations sur ce qui est nécessaire pour les autres types : [recherchez ce que le sensibles Types d’informations](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

