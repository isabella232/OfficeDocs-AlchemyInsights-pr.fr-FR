---
title: Résoudre les problèmes de l’inscription des appareils Android dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939346"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Résoudre les problèmes de l’inscription des appareils Android dans Microsoft Intune

Passez en revue les ressources répertoriées ci-dessous pour résoudre le problème maintenant.
  
Certains problèmes courants et les étapes de résolution :
  
 **Périphérique ne chiffré pas d’erreur dans le portail d’entreprise :** De nouvelles versions de Android, notamment commençant par 7.0, code secret démarrage pour vous assurer que votre périphérique est entièrement chiffré. Solutions courantes sont pour activer un code confidentiel de démarrage ou entièrement chiffrer le périphérique. Passez en revue [ce document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pour plus d’informations. 
  
 **Échouent vérifier avec le service Intune ou affichage sous la forme « Incorrecte du rapport » dans la console d’administration Intune :** Certains 4.4 Samsung et 5.5 périphériques peut ne pas vérifier dans le service. Il existe 3 solutions possibles à ce problème : 
  
1. Ouvrez manuellement l’application Intune portail d’entreprise, qui lance automatiquement une synchronisation du périphérique.
    
2. Mettre à jour l’appareil Android 6.0 ou version ultérieure.
    
3. Désactiver le Gestionnaire d’actives Samsung à la gestion du portail d’entreprise Intune. Passez en revue [ce document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pour plus d’informations sur ces problèmes et les solutions. 
    
 **Type de licence utilisateur incorrect** ou **erreur nom utilisateur non reconnu :** l’utilisateur doit être attribué une licence Intune ou EMS. Passez en revue ces documents pour attribuer une licence par le biais de : portail centre d’administration Office ou Azure. 
  
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utiliser le [Portail de résolution des problèmes de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscription courantes. Passez en revue [ce document](https://docs.microsoft.com/intune/help-desk-operators) pour plus d’informations. 
    
2. Passez en revue [ce document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pour obtenir la liste des erreurs courantes qui empêchent l’inscription et les résolutions à chacun. 
    
3. [Apprenez à inscrire les appareils Android dans Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

