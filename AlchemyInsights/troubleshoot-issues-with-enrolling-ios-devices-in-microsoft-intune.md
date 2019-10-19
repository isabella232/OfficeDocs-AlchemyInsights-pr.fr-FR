---
title: Résoudre les problèmes liés à l’enregistrement d’appareils iOS dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506925"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Résoudre les problèmes liés à l’enregistrement d’appareils iOS dans Microsoft Intune

Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant. 
  
Les messages d’erreur courants et les étapes de résolution sont les suivants :
  
- **Seuil d’appareil atteint** L’utilisateur dispose de plus d’appareils que la limite de l’appareil. Passez en revue ces documents pour [supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou [modifier la limite du périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ce service n’est pas pris en charge. Aucune stratégie d’inscriptions :** le service de notification d’envoi de message Apple (APNs) doit être configuré ou renouvelé. Consultez [ce document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la façon de procéder. 
    
- **Type de licence utilisateur non valide ou nom d’utilisateur non reconnu :** Une licence Intune ou EMS doit être attribuée à l’utilisateur. Passez en revue ces documents pour attribuer une licence via : [Centre d’administration Office](https://docs.microsoft.com/intune/licenses-assign) ou [portail Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants. Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Consultez ces documents pour obtenir la liste des erreurs courantes qui empêchent l’inscription et la résolution de chacune d’elles : [Guide de dépannage](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [Dépannage doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Découvrez comment inscrire des appareils iOS dans Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

