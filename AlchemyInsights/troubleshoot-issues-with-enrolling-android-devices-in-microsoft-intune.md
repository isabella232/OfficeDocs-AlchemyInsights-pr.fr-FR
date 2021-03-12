---
title: Résoudre les problèmes d’inscription d’appareils Android dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708996"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6311b-102">Résoudre les problèmes d’inscription d’appareils Android dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6311b-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6311b-103">Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant.</span><span class="sxs-lookup"><span data-stu-id="6311b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6311b-104">Quelques problèmes courants et étapes de résolution :</span><span class="sxs-lookup"><span data-stu-id="6311b-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6311b-105">**Erreur d’appareil non chiffré dans le portail d’entreprise :** Les versions plus récentes d’Android, en particulier à partir de la version v7.0, nécessitent un code secret de démarrage pour s’assurer que votre appareil est entièrement chiffré.</span><span class="sxs-lookup"><span data-stu-id="6311b-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="6311b-106">Les solutions courantes sont d’activer un code confidentiel de démarrage ou de chiffrer entièrement l’appareil.</span><span class="sxs-lookup"><span data-stu-id="6311b-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="6311b-107">Pour plus [d’informations,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="6311b-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="6311b-108">Les appareils ne parviennent pas à s’enregistrer avec le service Intune ou s’affichent comme « Défectueux » dans la **console d’administration Intune :** Certains appareils Samsung 4.4 et 5.5 peuvent ne pas être connectés au service.</span><span class="sxs-lookup"><span data-stu-id="6311b-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="6311b-109">Il existe 3 solutions possibles à ce problème :</span><span class="sxs-lookup"><span data-stu-id="6311b-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="6311b-110">Ouvrez manuellement l’application Portail d’entreprise Intune, qui lancera automatiquement une synchronisation d’appareil.</span><span class="sxs-lookup"><span data-stu-id="6311b-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="6311b-111">Mettez à jour l’appareil vers Android 6.0 ou version supérieure.</span><span class="sxs-lookup"><span data-stu-id="6311b-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="6311b-112">Désactivez Samsung Smart Manager de la gestion du portail d’entreprise Intune.</span><span class="sxs-lookup"><span data-stu-id="6311b-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="6311b-113">Pour [plus d’informations](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) sur ces problèmes et leurs résolutions, examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="6311b-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="6311b-114">**Type de licence utilisateur non** valide ou erreur de nom d’utilisateur non reconnu **:** une licence Intune ou EMS doit être attribuée à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6311b-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6311b-115">Examinez ces documents pour attribuer une licence par le biais du Centre d’administration Office ou du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="6311b-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="6311b-116">Ressources supplémentaires pour vous aider à résoudre votre problème :</span><span class="sxs-lookup"><span data-stu-id="6311b-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6311b-117">Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d’inscription courants.</span><span class="sxs-lookup"><span data-stu-id="6311b-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6311b-118">Pour [plus d’informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document.</span><span class="sxs-lookup"><span data-stu-id="6311b-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="6311b-119">Examinez [ce document pour](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) obtenir la liste des erreurs courantes qui empêchent l’inscription et les résolutions à chacune d’elles.</span><span class="sxs-lookup"><span data-stu-id="6311b-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="6311b-120">[Découvrez comment inscrire des appareils Android dans Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="6311b-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
