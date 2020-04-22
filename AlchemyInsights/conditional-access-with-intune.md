---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706019"
---
# <a name="conditional-access-with-intune"></a>Accès conditionnel avec Intune

L’utilisation de l' **accès conditionnel** avec Intune nécessite 3 étapes : 
  
- Créer une **stratégie d’accès conditionnel** qui définit les ressources à protéger et les conditions à respecter pour accéder à ces ressources. Par exemple, un appareil doit être conforme avant d’accéder à la messagerie d’entreprise. 
    
- Créez une **stratégie de conformité** pour définir les paramètres qui doivent être satisfaits pour que l’appareil soit considéré comme conforme. Par exemple, un appareil doit avoir un code confidentiel d’au moins 6 chiffres avant d’être considéré comme conforme. 
    
- S’assurer que les stratégies de **conformité** et les **stratégies d’accès conditionnel** sont ciblées pour les groupes d’utilisateurs souhaités. Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory. 
    
En savoir plus :
  
- [Meilleures pratiques en matière d’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Prise en main de l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

