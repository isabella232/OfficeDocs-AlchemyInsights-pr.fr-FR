---
title: Résoudre les problèmes d’inscription d’appareils Windows dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708888"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="c3f8e-102">Résoudre les problèmes d’inscription d’appareils Windows dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c3f8e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="c3f8e-103">Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c3f8e-104">Voici quelques messages d’erreur courants et les étapes de résolution :</span><span class="sxs-lookup"><span data-stu-id="c3f8e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="c3f8e-105">**Le logiciel ne peut pas être installé, 0x80cf4017 :** Le certificat de votre compte a expiré.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="c3f8e-106">Téléchargez à nouveau le package logiciel client PC dans la console d’administration Intune.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="c3f8e-107">Pour plus d’informations, examinez cette documentation.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="c3f8e-108">**Code d'0x801c0003 :** L’erreur peut se produire dans les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="c3f8e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="c3f8e-109">L’utilisateur a plus d’appareils inscrits que la limite d’appareils.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c3f8e-110">Examinez ces documents pour [supprimer un appareil ou](https://docs.microsoft.com/intune/devices-wipe) modifier la limite de [l’appareil.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="c3f8e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="c3f8e-111">« Les utilisateurs peuvent joindre des appareils à Azure AD » est définie sur « aucun ».</span><span class="sxs-lookup"><span data-stu-id="c3f8e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="c3f8e-112">Définissez-la sur tous les utilisateurs ou sélectionnez-les.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-112">Set it to all or select users.</span></span> <span data-ttu-id="c3f8e-113">Pour plus [d’informations,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) examinez cette documentation.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="c3f8e-114">L’appareil est déjà inscrit par un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="c3f8e-115">Si c’est le cas, supprimez l’appareil de la console Azure Intune ou désinscrissez manuellement l’appareil avant d’essayer à nouveau.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="c3f8e-116">L’appareil est Windows 10 Famille.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="c3f8e-117">Seules les SSO Windows 10 Professionnel, Éducation et Entreprise peuvent rejoindre Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="c3f8e-118">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="c3f8e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="c3f8e-119">Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d’inscription courants.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c3f8e-120">Pour [plus d’informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="c3f8e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="c3f8e-121">Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c3f8e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="c3f8e-122">[Découvrez comment inscrire des appareils Windows dans Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="c3f8e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
