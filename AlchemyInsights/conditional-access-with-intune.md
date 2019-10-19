---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504992"
---
# <a name="conditional-access-with-intune"></a>Accès conditionnel avec Intune

L’utilisation de l' **accès conditionnel** avec Intune nécessite 3 étapes : 
  
- Créer une **stratégie d’accès conditionnel** qui définit les ressources à protéger et les conditions à respecter pour accéder à ces ressources. Par exemple, un appareil doit être conforme avant d’accéder à la messagerie d’entreprise. 
    
- Créez une **stratégie de conformité** pour définir les paramètres qui doivent être satisfaits pour que l’appareil soit considéré comme conforme. Par exemple, un appareil doit avoir un code confidentiel d’au moins 6 chiffres avant d’être considéré comme conforme. 
    
- S’assurer que les stratégies de **conformité** et les **stratégies d’accès conditionnel** sont ciblées pour les groupes d’utilisateurs souhaités. Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory. 
    
En savoir plus :
  
- [Meilleures pratiques en matière d’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Prise en main de l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

