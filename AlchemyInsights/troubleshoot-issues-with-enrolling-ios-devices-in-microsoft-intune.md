---
title: Résoudre les problèmes d'inscription d'appareils iOS dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823461"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Résoudre les problèmes d'inscription d'appareils iOS dans Microsoft Intune

Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant. 
  
Voici quelques messages d'erreur courants et les étapes de résolution :
  
- **Limite d'appareil atteinte** L'utilisateur a plus d'appareils inscrits que la limite d'appareils. Examinez ces documents pour [supprimer un appareil ou](https://docs.microsoft.com/intune/devices-wipe) modifier la limite de [l'appareil.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ce service n'est pas pris en charge. Aucune stratégie d'inscription :** le service de notification Push Apple (APNS) doit être configuré ou renouvelé. Examinez [ce document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la façon de le faire. 
    
- **Type de licence utilisateur non valide ou nom d'utilisateur non reconnu :** Une licence Intune ou EMS doit être attribuée à l'utilisateur. Examinez ces documents pour attribuer une licence par le biais du Centre [d'administration Office](https://docs.microsoft.com/intune/licenses-assign) ou [du portail Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d'inscription courants. Pour [plus d'informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document. 
    
2. Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Découvrez comment inscrire des appareils iOS dans Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

