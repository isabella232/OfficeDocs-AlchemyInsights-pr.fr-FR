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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2aa18-102">Résoudre les problèmes liés à l’enregistrement d’appareils iOS dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2aa18-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2aa18-103">Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant.</span><span class="sxs-lookup"><span data-stu-id="2aa18-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2aa18-104">Les messages d’erreur courants et les étapes de résolution sont les suivants :</span><span class="sxs-lookup"><span data-stu-id="2aa18-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2aa18-105">**Seuil d’appareil atteint** L’utilisateur dispose de plus d’appareils que la limite de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="2aa18-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2aa18-106">Passez en revue ces documents pour [supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou [modifier la limite du périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2aa18-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2aa18-107">**Ce service n’est pas pris en charge. Aucune stratégie d’inscriptions :** le service de notification d’envoi de message Apple (APNs) doit être configuré ou renouvelé.</span><span class="sxs-lookup"><span data-stu-id="2aa18-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="2aa18-108">Consultez [ce document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pour obtenir des instructions sur la façon de procéder.</span><span class="sxs-lookup"><span data-stu-id="2aa18-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2aa18-109">**Type de licence utilisateur non valide ou nom d’utilisateur non reconnu :** Une licence Intune ou EMS doit être attribuée à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2aa18-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2aa18-110">Passez en revue ces documents pour attribuer une licence via : [Centre d’administration Office](https://docs.microsoft.com/intune/licenses-assign) ou [portail Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="2aa18-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2aa18-111">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="2aa18-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2aa18-112">Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants.</span><span class="sxs-lookup"><span data-stu-id="2aa18-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2aa18-113">Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="2aa18-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2aa18-114">Consultez ces documents pour obtenir la liste des erreurs courantes qui empêchent l’inscription et la résolution de chacune d’elles : [Guide de dépannage](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) et [Dépannage doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2aa18-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2aa18-115">[Découvrez comment inscrire des appareils iOS dans Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="2aa18-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

