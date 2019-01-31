---
title: Résoudre les problèmes de l’inscription des appareils Android dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655881"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="996ef-102">Résoudre les problèmes de l’inscription des appareils Android dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="996ef-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="996ef-103">Passez en revue les ressources répertoriées ci-dessous pour résoudre le problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="996ef-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="996ef-104">Certains problèmes courants et les étapes de résolution :</span><span class="sxs-lookup"><span data-stu-id="996ef-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="996ef-p101">**Périphérique ne chiffré pas d’erreur dans le portail d’entreprise :** De nouvelles versions de Android, notamment commençant par 7.0, code secret démarrage pour vous assurer que votre périphérique est entièrement chiffré. Solutions courantes sont pour activer un code confidentiel de démarrage ou entièrement chiffrer le périphérique. Passez en revue [ce document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="996ef-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="996ef-p102">**Échouent vérifier avec le service Intune ou affichage sous la forme « Incorrecte du rapport » dans la console d’administration Intune :** Certains 4.4 Samsung et 5.5 périphériques peut ne pas vérifier dans le service. Il existe 3 solutions possibles à ce problème :</span><span class="sxs-lookup"><span data-stu-id="996ef-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="996ef-110">Ouvrez manuellement l’application Intune portail d’entreprise, qui lance automatiquement une synchronisation du périphérique.</span><span class="sxs-lookup"><span data-stu-id="996ef-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="996ef-111">Mettre à jour l’appareil Android 6.0 ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="996ef-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="996ef-p103">Désactiver le Gestionnaire d’actives Samsung à la gestion du portail d’entreprise Intune. Passez en revue [ce document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pour plus d’informations sur ces problèmes et les solutions.</span><span class="sxs-lookup"><span data-stu-id="996ef-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="996ef-p104">**Type de licence utilisateur incorrect** ou **erreur nom utilisateur non reconnu :** l’utilisateur doit être attribué une licence Intune ou EMS. Passez en revue ces documents pour attribuer une licence par le biais de : portail centre d’administration Office ou Azure.</span><span class="sxs-lookup"><span data-stu-id="996ef-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="996ef-116">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="996ef-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="996ef-p105">Utiliser le [Portail de résolution des problèmes de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscription courantes. Passez en revue [ce document](https://docs.microsoft.com/intune/help-desk-operators) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="996ef-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="996ef-119">Passez en revue [ce document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pour obtenir la liste des erreurs courantes qui empêchent l’inscription et les résolutions à chacun.</span><span class="sxs-lookup"><span data-stu-id="996ef-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="996ef-120">[Apprenez à inscrire les appareils Android dans Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="996ef-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

