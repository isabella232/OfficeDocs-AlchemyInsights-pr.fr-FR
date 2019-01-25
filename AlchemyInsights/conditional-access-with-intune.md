---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469182"
---
# <a name="conditional-access-with-intune"></a>Accès conditionnel avec Intune

À l’aide de **L’accès conditionnel** avec Intune requiert 3 comme suit : 
  
- Créer une **Stratégie d’accès conditionnel** qui définit les ressources qui sont protégés, et les conditions qui doivent être remplies pour accéder à ces ressources. Par exemple, un périphérique doit être conforme avant d’accéder à la messagerie d’entreprise. 
    
- Créer une **Stratégie de conformité** pour définir les paramètres qui doivent être remplis avant que le périphérique est considéré comme conforme. Par exemple, un périphérique doit avoir un code confidentiel d’au moins 6 chiffres est considéré comme conforme. 
    
- Vérifier les **Stratégies de conformité** et **Les stratégies d’accès conditionnel** destinées à des groupes d’utilisateurs requis. Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory. 
    
En savoir plus
  
- [Meilleures pratiques en matière de conditionnelle accès](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [Mise en route avec accès conditionnel](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

