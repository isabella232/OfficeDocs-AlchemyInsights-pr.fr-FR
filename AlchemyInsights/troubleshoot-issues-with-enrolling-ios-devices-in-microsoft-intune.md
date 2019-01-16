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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288850"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2c42b-102">Résoudre les problèmes de l’inscription des appareils iOS dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2c42b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2c42b-103">Passez en revue les ressources répertoriées ci-dessous pour résoudre le problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="2c42b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2c42b-104">Certains messages d’erreur courants et les étapes de résolution :</span><span class="sxs-lookup"><span data-stu-id="2c42b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2c42b-p101">**Cap périphérique atteint** L’utilisateur dispose de plusieurs périphériques inscrits à la limite du périphérique. Passez en revue ces documents pour [Supprimer un périphérique](https://docs.microsoft.com/en-us/intune/devices-wipe) ou de [Modifier la limite de périphérique](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2c42b-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2c42b-p102">**Ce Service n’est pas pris en charge. Aucune stratégie d’inscription :** Service de Notification Push Apple (APNS) doit être configuré ou renouvelée. Passez en revue [ce document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la procédure à suivre.</span><span class="sxs-lookup"><span data-stu-id="2c42b-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2c42b-p103">**Type de licence utilisateur non valide ou le nom d’utilisateur non reconnu :** L’utilisateur doit être attribué une licence Intune ou EMS. Passez en revue ces documents pour attribuer une licence par le biais de : [Centre d’administration Office](https://docs.microsoft.com/en-us/intune/licenses-assign) ou [portail Azure](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="2c42b-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2c42b-111">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="2c42b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2c42b-p104">Utiliser le [Portail de résolution des problèmes de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscription courantes. Passez en revue [ce document](https://docs.microsoft.com/en-us/intune/help-desk-operators) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="2c42b-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2c42b-114">Passez en revue ces documents pour la liste des erreurs qui empêchent l’inscription et les résolutions à chacun : [guide de résolution des problèmes](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [dépannage doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2c42b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2c42b-115">[Apprenez à inscrire les appareils iOS dans Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="2c42b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

