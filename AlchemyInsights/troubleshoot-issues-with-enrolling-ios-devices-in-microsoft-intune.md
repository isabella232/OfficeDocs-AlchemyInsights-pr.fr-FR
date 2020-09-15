---
title: Résoudre les problèmes liés à l’enregistrement d’appareils iOS dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669246"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Résoudre les problèmes liés à l’enregistrement d’appareils iOS dans Microsoft Intune

Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant. 
  
Les messages d’erreur courants et les étapes de résolution sont les suivants :
  
- **Seuil d’appareil atteint** L’utilisateur dispose de plus d’appareils que la limite de l’appareil. Passez en revue ces documents pour [supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou [modifier la limite du périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ce service n’est pas pris en charge. Aucune stratégie d’inscriptions :** le service de notification d’envoi de message Apple (APNs) doit être configuré ou renouvelé. Consultez [ce document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la façon de procéder. 
    
- **Type de licence utilisateur non valide ou nom d’utilisateur non reconnu :** Une licence Intune ou EMS doit être attribuée à l’utilisateur. Passez en revue ces documents pour attribuer une licence via : [Centre d’administration Office](https://docs.microsoft.com/intune/licenses-assign) ou [portail Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants. Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Découvrez comment inscrire des appareils iOS dans Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

