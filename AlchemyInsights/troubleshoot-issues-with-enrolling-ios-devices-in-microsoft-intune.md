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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="7e53d-102">Résoudre les problèmes d'inscription d'appareils iOS dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7e53d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="7e53d-103">Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="7e53d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="7e53d-104">Voici quelques messages d'erreur courants et les étapes de résolution :</span><span class="sxs-lookup"><span data-stu-id="7e53d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="7e53d-105">**Limite d'appareil atteinte** L'utilisateur a plus d'appareils inscrits que la limite d'appareils.</span><span class="sxs-lookup"><span data-stu-id="7e53d-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7e53d-106">Examinez ces documents pour [supprimer un appareil ou](https://docs.microsoft.com/intune/devices-wipe) modifier la limite de [l'appareil.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7e53d-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="7e53d-107">**Ce service n'est pas pris en charge. Aucune stratégie d'inscription :** le service de notification Push Apple (APNS) doit être configuré ou renouvelé.</span><span class="sxs-lookup"><span data-stu-id="7e53d-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="7e53d-108">Examinez [ce document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la façon de le faire.</span><span class="sxs-lookup"><span data-stu-id="7e53d-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="7e53d-109">**Type de licence utilisateur non valide ou nom d'utilisateur non reconnu :** Une licence Intune ou EMS doit être attribuée à l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7e53d-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="7e53d-110">Examinez ces documents pour attribuer une licence par le biais du Centre [d'administration Office](https://docs.microsoft.com/intune/licenses-assign) ou [du portail Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="7e53d-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="7e53d-111">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="7e53d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7e53d-112">Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d'inscription courants.</span><span class="sxs-lookup"><span data-stu-id="7e53d-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7e53d-113">Pour [plus d'informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="7e53d-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="7e53d-114">Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="7e53d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="7e53d-115">[Découvrez comment inscrire des appareils iOS dans Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="7e53d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

