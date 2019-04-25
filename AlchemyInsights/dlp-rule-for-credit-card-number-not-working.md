---
title: La règle DLP pour le numéro de carte de crédit ne fonctionne pas
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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404489"
---
Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de carte bancaire** lors de l'utilisation d'un type d'informations sensibles DLP dans O365? Si c'est le cas, assurez-vous que votre contenu contient les informations nécessaires pour déclencher la stratégie DLP lors de son évaluation. Par exemple, pour une **stratégie de carte de crédit** configurée avec un niveau de confiance de 85%, les éléments suivants sont évalués et doivent être détectés pour le déclenchement de la règle: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chiffres qui peuvent être mis en forme ou non (dddddddddddddddd) et doivent réussir le test Luhn. 
    
- **[Modèle:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Modèle très complexe et robuste qui détecte les cartes de toutes les principales marques dans le monde, notamment les cartes Visa, MasterCard, Discover Card, JCB, American Express, les cartes cadeaux et les cartes dîner. 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Oui, la somme de contrôle Luhn 
    
- **[Définition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Une stratégie DLP est sûre à 85% d'avoir détecté ce type d'informations sensibles si, dans une proximité de 300 caractères: 
    
  - La fonction Func_credit_card trouve un contenu qui correspond au modèle.
    
  - L’une des affirmations suivantes est vraie : 
    
  - Un mot clé figurant dans la liste Keyword_cc_verification est trouvé.
    
  - Un mot clé depuis Keyword_cc_name est trouvé.
    
  - La fonction Func_expiration_date trouve une date au format correct.
    
  - Le checksum passe
    
    Par exemple, l'exemple suivant se déclenche pour une stratégie de numéro de carte de crédit DLP:
    
  - Visa: 4485 3647 3952 7352 
    
  - Date d'expiration: 2/2009
    
Pour plus d'informations sur les éléments requis pour la détection d'un **numéro de carte de crédit** pour votre contenu, reportez-vous à la section suivante de cet article: [ce que recherche les types d'informations sensibles pour la carte de crédit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
À l'aide d'un type d'informations sensibles intégré différent, consultez l'article suivant pour obtenir des informations sur les éléments requis pour les autres types: [ce que recherche les types d'informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

