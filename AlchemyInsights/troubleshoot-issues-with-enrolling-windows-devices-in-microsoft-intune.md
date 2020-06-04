---
title: Résoudre les problèmes liés à l’inscrire des appareils Windows dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665830"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="b501d-102">Résoudre les problèmes liés à l’inscrire des appareils Windows dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b501d-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="b501d-103">Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant.</span><span class="sxs-lookup"><span data-stu-id="b501d-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b501d-104">Les messages d’erreur courants et les étapes de résolution sont les suivants :</span><span class="sxs-lookup"><span data-stu-id="b501d-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="b501d-105">**Le logiciel ne peut pas être installé, 0x80cf4017 :** Votre certificat de compte a expiré.</span><span class="sxs-lookup"><span data-stu-id="b501d-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="b501d-106">Téléchargez de nouveau le package logiciel client PC dans la console d’administration Intune.</span><span class="sxs-lookup"><span data-stu-id="b501d-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="b501d-107">Pour plus d’informations, consultez cette documentation.</span><span class="sxs-lookup"><span data-stu-id="b501d-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="b501d-108">**Code d’erreur 0x801c0003 :** L’erreur peut se produire dans les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="b501d-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="b501d-109">L’utilisateur dispose de plus d’appareils que la limite de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="b501d-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b501d-110">Passez en revue ces documents pour [supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou [modifier la limite du périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b501d-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="b501d-111">« Les utilisateurs peuvent rejoindre les appareils sur Azure AD » est défini sur « aucun ».</span><span class="sxs-lookup"><span data-stu-id="b501d-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="b501d-112">Définissez-la sur tous les utilisateurs ou sélectionnez-les.</span><span class="sxs-lookup"><span data-stu-id="b501d-112">Set it to all or select users.</span></span> <span data-ttu-id="b501d-113">Pour plus d’informations, consultez [cette documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="b501d-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="b501d-114">L’appareil est déjà déployé par un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b501d-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="b501d-115">Si c’est le cas, supprimez l’appareil de la console Azure Intune ou désinscrivez manuellement l’appareil, puis réessayez.</span><span class="sxs-lookup"><span data-stu-id="b501d-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="b501d-116">Le périphérique est Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="b501d-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="b501d-117">Seuls Windows 10 professionnel, les SKU éducation et entreprise peuvent rejoindre Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b501d-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="b501d-118">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="b501d-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="b501d-119">Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants.</span><span class="sxs-lookup"><span data-stu-id="b501d-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b501d-120">Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="b501d-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="b501d-121">Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b501d-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="b501d-122">[Découvrez comment inscrire des appareils Windows dans Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="b501d-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
