---
title: Résoudre les problèmes liés à l’enregistrement d’appareils Android dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759618"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="f566f-102">Résoudre les problèmes liés à l’enregistrement d’appareils Android dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f566f-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="f566f-103">Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant.</span><span class="sxs-lookup"><span data-stu-id="f566f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f566f-104">Voici quelques étapes de résolution et de problèmes courants :</span><span class="sxs-lookup"><span data-stu-id="f566f-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="f566f-105">**Erreur de périphérique non chiffré dans le portail d’entreprise :** Les versions plus récentes d’Android, en particulier à partir de la version 7.0, nécessitent un code secret de démarrage pour s’assurer que votre appareil est entièrement chiffré.</span><span class="sxs-lookup"><span data-stu-id="f566f-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="f566f-106">Les solutions courantes sont l’activation d’un code confidentiel de démarrage ou le chiffrement complet de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="f566f-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="f566f-107">Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="f566f-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="f566f-108">Les **appareils ne parviennent pas à archiver avec le service Intune ou s’affichent comme « défectueux » dans la console d’administration Intune :** Certains appareils Samsung 4,4 et 5,5 ne peuvent pas archiver le service.</span><span class="sxs-lookup"><span data-stu-id="f566f-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="f566f-109">Il existe trois solutions possibles à ce problème :</span><span class="sxs-lookup"><span data-stu-id="f566f-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="f566f-110">Ouvrez manuellement l’application portail d’entreprise Intune, qui lance automatiquement une synchronisation d’appareil.</span><span class="sxs-lookup"><span data-stu-id="f566f-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="f566f-111">Mettez à jour l’appareil vers Android 6,0 ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f566f-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="f566f-112">Désactivez le Gestionnaire intelligent Samsung de la gestion du portail d’entreprise Intune.</span><span class="sxs-lookup"><span data-stu-id="f566f-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="f566f-113">Consultez [ce document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pour plus d’informations sur ces problèmes et solutions.</span><span class="sxs-lookup"><span data-stu-id="f566f-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="f566f-114">**Type de licence utilisateur non valide** ou **nom d’utilisateur non reconnu :** l’utilisateur doit se voir attribuer une licence Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="f566f-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f566f-115">Passez en revue ces documents pour attribuer une licence via : Centre d’administration Office ou portail Azure.</span><span class="sxs-lookup"><span data-stu-id="f566f-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="f566f-116">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="f566f-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f566f-117">Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants.</span><span class="sxs-lookup"><span data-stu-id="f566f-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f566f-118">Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="f566f-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f566f-119">Consultez [ce document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pour obtenir la liste des erreurs courantes qui empêchent l’inscription et la résolution de chacune d’elles.</span><span class="sxs-lookup"><span data-stu-id="f566f-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="f566f-120">[Découvrez comment inscrire des appareils Android dans Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="f566f-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
