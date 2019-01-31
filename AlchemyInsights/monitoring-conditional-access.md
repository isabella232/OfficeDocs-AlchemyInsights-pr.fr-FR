---
title: Surveillance de l’accès conditionnel
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656565"
---
# <a name="monitoring-conditional-access"></a>Surveillance de l’accès conditionnel

Les utilisateurs ciblés avec accès conditionnel reçoit un message électronique de notification si elles ne remplissent pas les conditions d’accès de votre organisation. Pour résoudre, nous vous recommandons d’une ou plusieurs des solutions suivantes :
  
- Si le périphérique est censé être inscrit, informer l’utilisateur à accéder à l’application de portail d’entreprise et vérifiez qu’il apparaît dans le portail d’entreprise. Le cas contraire, l’utilisateur doit s’inscrire l’appareil.
    
- Dans le portail Azure, accédez à **Intune \> conformité périphérique**. Sous **Moniteur** , cliquez sur **la conformité du périphérique**. Afficher l’état de conformité de périphérique pour vérifier que le périphérique de l’utilisateur est marqué comme conforme. 
    
- Dans le portail Azure, accédez à **Intune \> conformité périphérique**. Sous **Gérer**, cliquez sur **stratégies**. Dans la liste des stratégies de conformité, vérifiez qu’un profil est attribué au périphérique de l’utilisateur. Si aucun profil n’est assigné, Intune ne sera pas en mesure de confirmer le statut de conformité de l’appareil. 
    
- Modifier l’affectation d’accès conditionnel de l’utilisateur.
    
1. Dans le portail Azure, accédez à **Intune \> accès conditionnel \> stratégies**
    
2. Sélectionnez une stratégie dans la liste
    
3. Cliquez sur **utilisateurs et groupes**
    
4. Pour cibler une stratégie à une personne spécifique, ajoutez-les à la liste **d’inclusion** . Pour vous assurer qu’une personne est omise de la stratégie, les ajouter à la liste **à exclure** . 
    
En savoir plus : [comment surveiller l’accès conditionnel périphériques](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

