---
title: Problèmes de suppression d’un appareil désintôt ou désaffecté de l’inventaire des appareils
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319173"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="5b5d4-102">Problèmes de suppression d’un appareil désintôt ou désaffecté de l’inventaire des appareils</span><span class="sxs-lookup"><span data-stu-id="5b5d4-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="5b5d4-103">Microsoft Defender pour le point de terminaison n’autorise pas actuellement la suppression manuelle de l’enregistrement d’appareil d’un appareil désintôt ou désaffecté de l’inventaire des appareils.</span><span class="sxs-lookup"><span data-stu-id="5b5d4-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="5b5d4-104">Pour des raisons de sécurité, l’appareil reste dans le portail en tant qu’enregistrement historique pendant 180 jours au plus.</span><span class="sxs-lookup"><span data-stu-id="5b5d4-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="5b5d4-105">Toutefois, les données de l’appareil sont purgées en fonction de votre période de rétention configurée.</span><span class="sxs-lookup"><span data-stu-id="5b5d4-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="5b5d4-106">**Remarque :** Un appareil désintté ou désaffecté passe automatiquement à l’état **Inactif** au bout de sept jours.</span><span class="sxs-lookup"><span data-stu-id="5b5d4-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="5b5d4-107">En outre, les appareils non actifs au cours des 30 derniers jours ne sont pas pris en compte dans les données qui reflètent le score d’exposition aux menaces et à la gestion des vulnérabilités de votre organisation ou le Degré de sécurisation Microsoft pour les appareils.</span><span class="sxs-lookup"><span data-stu-id="5b5d4-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="5b5d4-108">Si vous ne souhaitez toujours pas voir certains appareils dans l’affichage Inventaire des appareils, essayez de placer une balise d’appareil pour filtrer l’appareil désaffecté de l’affichage Inventaire des appareils.</span><span class="sxs-lookup"><span data-stu-id="5b5d4-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="5b5d4-109">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="5b5d4-109">For more information, see:</span></span>

[<span data-ttu-id="5b5d4-110">Hors-carte des appareils à partir du service Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="5b5d4-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="5b5d4-111">Score d’exposition dans la gestion des menaces et des vulnérabilités</span><span class="sxs-lookup"><span data-stu-id="5b5d4-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="5b5d4-112">Corriger les capteurs défectueux dans Microsoft Defender pour le point de terminaison</span><span class="sxs-lookup"><span data-stu-id="5b5d4-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="5b5d4-113">Utilisation efficace du balisage (partie 1)</span><span class="sxs-lookup"><span data-stu-id="5b5d4-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="5b5d4-114">Utilisation efficace du balisage (partie 2)</span><span class="sxs-lookup"><span data-stu-id="5b5d4-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="5b5d4-115">Utilisation efficace du balisage (partie 3)</span><span class="sxs-lookup"><span data-stu-id="5b5d4-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




