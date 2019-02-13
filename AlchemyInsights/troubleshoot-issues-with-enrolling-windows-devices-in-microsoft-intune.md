---
title: Résoudre les problèmes de l’inscription des périphériques Windows Intune Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934774"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d5b8c-102">Résoudre les problèmes de l’inscription des périphériques Windows Intune Microsoft</span><span class="sxs-lookup"><span data-stu-id="d5b8c-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d5b8c-103">Passez en revue les ressources répertoriées ci-dessous pour résoudre le problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="d5b8c-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d5b8c-104">Certains messages d’erreur courants et les étapes de résolution :</span><span class="sxs-lookup"><span data-stu-id="d5b8c-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d5b8c-p101">**Ne peut pas être installé le logiciel, 0x80cf4017 :** Votre certificat de compte a expiré. Télécharger le logiciel PC Client dans la Console d’administration Intune à nouveau. Consultez cette documentation pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="d5b8c-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="d5b8c-108">**Code d’erreur 0x801c0003 :** L’erreur peut se produire dans les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="d5b8c-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="d5b8c-p102">L’utilisateur dispose de plusieurs périphériques inscrits à la limite du périphérique. Passez en revue ces documents pour [Supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou de [Modifier la limite de périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d5b8c-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="d5b8c-p103">« Les utilisateurs peuvent se joindre à périphériques pour Azure AD » est définie sur « none ». Valeur tous ou sélectionnez utilisateurs. Passez en revue [cette documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="d5b8c-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="d5b8c-p104">Le périphérique est déjà inscrit par un autre utilisateur. Si tel est le cas, supprimez le périphérique à partir de la console d’Azure Intune ou unenroll manuellement le périphérique avant de réessayer.</span><span class="sxs-lookup"><span data-stu-id="d5b8c-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="d5b8c-p105">Le périphérique est 10 d’accueil. Uniquement Windows 10 Pro, formation et SKU peuvent participer à Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d5b8c-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="d5b8c-118">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="d5b8c-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d5b8c-p106">Utiliser le [Portail de résolution des problèmes de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscription courantes. Passez en revue [ce document](https://docs.microsoft.com/intune/help-desk-operators) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="d5b8c-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d5b8c-121">Passez en revue ces documents pour la liste des erreurs qui empêchent l’inscription et les résolutions à chacun : [guide de résolution des problèmes](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [dépannage doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d5b8c-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="d5b8c-122">[Apprenez à inscrire des périphériques Windows Intune Microsoft](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="d5b8c-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

