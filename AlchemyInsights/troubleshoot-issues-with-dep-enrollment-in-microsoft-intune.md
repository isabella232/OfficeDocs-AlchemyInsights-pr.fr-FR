---
title: Résoudre les problèmes d'inscription de PDN dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 27abeafba5588ca74569ba6bebc5d940b767ea3f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824505"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="512c0-102">Résoudre les problèmes d'inscription de PDN dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="512c0-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="512c0-103">Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="512c0-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="512c0-104">Si l'appareil DEP ne parvient pas à s'inscrire et que l'authentification multifacteur (MFA) est activée, désactivez l'authentification multifacteur.</span><span class="sxs-lookup"><span data-stu-id="512c0-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="512c0-105">Actuellement, l' mbam n'est pas pris en charge pour l'inscription DEP</span><span class="sxs-lookup"><span data-stu-id="512c0-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="512c0-106">Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d'inscription courants.</span><span class="sxs-lookup"><span data-stu-id="512c0-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="512c0-107">Pour [plus d'informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="512c0-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="512c0-108">Examinez ces documents pour obtenir la liste des erreurs courantes qui empêchent l'inscription et les résolutions à chacune d'elles : [guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) de dépannage et document [de dépannage](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="512c0-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="512c0-109">[En savoir plus sur le programme d'inscription des appareils.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="512c0-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
