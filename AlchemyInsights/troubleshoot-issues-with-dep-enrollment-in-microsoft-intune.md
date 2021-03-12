---
title: Résoudre les problèmes d’inscription de PDN dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708708"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="cbf6f-102">Résoudre les problèmes d’inscription de PDN dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cbf6f-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="cbf6f-103">Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="cbf6f-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="cbf6f-104">Si l’appareil DEP ne parvient pas à s’inscrire et que l’authentification multifacteur (MFA) est activée, désactivez l’authentification multifacteur.</span><span class="sxs-lookup"><span data-stu-id="cbf6f-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="cbf6f-105">Actuellement, l' mbam n’est pas pris en charge pour l’inscription DEP</span><span class="sxs-lookup"><span data-stu-id="cbf6f-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="cbf6f-106">Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d’inscription courants.</span><span class="sxs-lookup"><span data-stu-id="cbf6f-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="cbf6f-107">Pour [plus d’informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="cbf6f-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="cbf6f-108">Examinez ces documents pour obtenir la liste des erreurs courantes qui empêchent l’inscription et les résolutions à chacune d’elles : [guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) de dépannage et document [de dépannage](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="cbf6f-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="cbf6f-109">[En savoir plus sur le programme d’inscription des appareils.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="cbf6f-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
