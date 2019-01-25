---
title: Résoudre les problèmes de l’inscription des appareils iOS dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469177"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Résoudre les problèmes de l’inscription des appareils iOS dans Microsoft Intune

Passez en revue les ressources répertoriées ci-dessous pour résoudre le problème maintenant. 
  
Certains messages d’erreur courants et les étapes de résolution :
  
- **Cap périphérique atteint** L’utilisateur dispose de plusieurs périphériques inscrits à la limite du périphérique. Passez en revue ces documents pour [Supprimer un périphérique](https://docs.microsoft.com/en-us/intune/devices-wipe) ou de [Modifier la limite de périphérique](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ce Service n’est pas pris en charge. Aucune stratégie d’inscription :** Service de Notification Push Apple (APNS) doit être configuré ou renouvelée. Passez en revue [ce document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la procédure à suivre. 
    
- **Type de licence utilisateur non valide ou le nom d’utilisateur non reconnu :** L’utilisateur doit être attribué une licence Intune ou EMS. Passez en revue ces documents pour attribuer une licence par le biais de : [Centre d’administration Office](https://docs.microsoft.com/en-us/intune/licenses-assign) ou [portail Azure](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utiliser le [Portail de résolution des problèmes de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscription courantes. Passez en revue [ce document](https://docs.microsoft.com/en-us/intune/help-desk-operators) pour plus d’informations. 
    
2. Passez en revue ces documents pour la liste des erreurs qui empêchent l’inscription et les résolutions à chacun : [guide de résolution des problèmes](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [dépannage doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Apprenez à inscrire les appareils iOS dans Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

