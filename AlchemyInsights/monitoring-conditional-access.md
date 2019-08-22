---
title: Surveillance de l’accès conditionnel
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538740"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Surveillance de l’accès conditionnel pour Exchange

Les utilisateurs ciblés avec l’accès conditionnel recevront un courrier électronique de notification s’ils ne répondent pas aux exigences d’accès de votre organisation. Pour résoudre ce qui suit, nous vous recommandons d’utiliser une ou plusieurs des solutions suivantes:
  
- Si le périphérique est présumé être inscrire, conseillez-lui d’accéder à l’application portail d’entreprise et de vérifier qu’il apparaît dans le portail d’entreprise. Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.
    
- Dans le portail Azure, accédez **à \> Intune Device Compliance**. Sous **analyse** , cliquez sur **conformité des appareils**. Affichez votre rapport de conformité des appareils pour vérifier que l’appareil de l’utilisateur est marqué comme étant compatible. 
    
- Dans le portail Azure, accédez **à \> Intune Device Compliance**. Sous **gérer**, cliquez sur **stratégies**. Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur. Si aucun profil n’est affecté, Intune ne pourra pas confirmer l’état de conformité de l’appareil. 
    
- Modifiez l’attribution d’accès conditionnel de l’utilisateur.
    
1. Dans le portail Azure, accéder **aux \> stratégies d' \> accès conditionnel Intune**
    
2. Sélectionner une stratégie dans la liste
    
3. Cliquez sur **utilisateurs et groupes**
    
4. Pour cibler une stratégie spécifique à une personne, ajoutez-la à la liste **inclure** . Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la liste d' **exclusion** . 
    
En savoir plus: [comment surveiller les appareils d’accès conditionnel](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

