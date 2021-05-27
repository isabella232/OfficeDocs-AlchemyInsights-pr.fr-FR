---
title: État des points de terminaison Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627232"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="23351-102">État des points de terminaison Defender</span><span class="sxs-lookup"><span data-stu-id="23351-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="23351-103">La vignette **Appareils avec problèmes de détection.** est située dans le tableau de bord opérations de sécurité.</span><span class="sxs-lookup"><span data-stu-id="23351-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="23351-104">Cette vignette fournit des informations sur la capacité de chaque appareil à fournir des données de détection à communiquer avec le service Defender pour point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="23351-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="23351-105">Elle indique le nombre d’appareils qui nécessitent une attention particulière et vous aide à identifier les appareils problématiques et à prendre des mesures pour les corriger.</span><span class="sxs-lookup"><span data-stu-id="23351-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="23351-106">Deux indicateurs d’état sur la vignette fournissent des informations sur le nombre d’appareils qui ne rapportent pas correctement au service :</span><span class="sxs-lookup"><span data-stu-id="23351-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="23351-107">**Mal configurés** Appareils qui peuvent signaler partiellement des données de détection au service Defender pour point de terminaison et qui peuvent présenter des erreurs de configuration devant être corrigées.</span><span class="sxs-lookup"><span data-stu-id="23351-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="23351-108">**Inactifs** Appareils qui ont cessé de rendre compte au service Defender pour le point de terminaison pendant plus de sept jours au cours du mois précédent.</span><span class="sxs-lookup"><span data-stu-id="23351-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="23351-109">En cliquant sur l'un des groupes, vous accédez à la liste Appareils, filtrée en fonction de vos choix.</span><span class="sxs-lookup"><span data-stu-id="23351-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="23351-110">Dans la liste Appareils, vous pouvez filtrer la liste d’état d’intégrité selon l’état suivant :</span><span class="sxs-lookup"><span data-stu-id="23351-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="23351-111">**Actifs** Appareils signalés activement au service Defender pour point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="23351-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="23351-112">**Mal configurés** Appareils qui peuvent signaler partiellement des données de détection au service Defender pour points de terminaison, mais présentent des erreurs de configuration devant être corrigées.</span><span class="sxs-lookup"><span data-stu-id="23351-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="23351-113">Les appareils mal configurés peuvent avoir l’un ou l’autre des problèmes suivants :</span><span class="sxs-lookup"><span data-stu-id="23351-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="23351-114">Aucune donnée de détection : les appareils ont arrêté d’envoyer des données de détection.</span><span class="sxs-lookup"><span data-stu-id="23351-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="23351-115">Des alertes limitées peuvent être déclenchées à partir de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="23351-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="23351-116">Communications altérées : la capacité à communiquer avec l’appareil est altérée.</span><span class="sxs-lookup"><span data-stu-id="23351-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="23351-117">Il est possible que l'envoi de fichiers pour une analyse approfondie, le blocage de fichiers, l'isolement de l'appareil du réseau et d'autres actions qui nécessitent une communication avec l'appareil ne fonctionnent pas.</span><span class="sxs-lookup"><span data-stu-id="23351-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="23351-118">**Inactifs** Appareils qui ont cessé de rendre compte au service Defender pour le point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="23351-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="23351-119">Vous pouvez télécharger la liste entière au format CSV à l'aide de la fonctionnalité Exporter.</span><span class="sxs-lookup"><span data-stu-id="23351-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="23351-120">Pour plus d’informations, consultez [Vérifier l'état d'intégrité de détection dans Microsoft Defender pour point de terminaison](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="23351-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="23351-121">Pour plus d’informations sur la cause de l’inactivité ou de la configuration d’un appareil, consultez [Corriger les détecteurs malsains dans Microsoft Defender pour point de terminaison](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="23351-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
