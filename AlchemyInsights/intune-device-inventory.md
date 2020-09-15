---
title: Inventaire des appareils Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667876"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="67ed5-102">Inventaire des appareils Intune</span><span class="sxs-lookup"><span data-stu-id="67ed5-102">Intune Device Inventory</span></span>

<span data-ttu-id="67ed5-103">Le panneau Appareils fournit à l’administrateur des informations sur les appareils sous gestion dans Intune sur une base par appareil.</span><span class="sxs-lookup"><span data-stu-id="67ed5-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="67ed5-104">Les informations présentées incluent les éléments suivants : matériel, applications détectées, état de conformité des appareils et état de configuration des appareils.</span><span class="sxs-lookup"><span data-stu-id="67ed5-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="67ed5-105">Les données d’inventaire du matériel et des applications découvertes sont collectées sur un cycle de 7 jours.</span><span class="sxs-lookup"><span data-stu-id="67ed5-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="67ed5-106">Les applications et les éléments spécifiques du matériel signalé diffèrent selon le système d’exploitation de l’appareil et selon que l’appareil est possédé ou d’une entreprise.</span><span class="sxs-lookup"><span data-stu-id="67ed5-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="67ed5-107">Pour plus d’informations, consultez [Afficher les détails de l’appareil dans Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="67ed5-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="67ed5-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="67ed5-108">**FAQ**</span></span>

<span data-ttu-id="67ed5-109">Q : je ne reçois aucune liste d’inventaire complète des applications présentes sur les appareils Windows inscrits sur Intune.</span><span class="sxs-lookup"><span data-stu-id="67ed5-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="67ed5-110">Pourquoi ?</span><span class="sxs-lookup"><span data-stu-id="67ed5-110">Why not?</span></span>

<span data-ttu-id="67ed5-111">R : pour le moment, seules les applications modernes sont répertoriées pour les PC Windows 10 identifiés en tant qu’appareils d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="67ed5-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="67ed5-112">Intune ne recueille pas d’informations sur les applications Win32 installées sur ces appareils.</span><span class="sxs-lookup"><span data-stu-id="67ed5-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="67ed5-113">Q : pourquoi les numéros de téléphone ne sont-ils pas collectés sur tous les appareils ?</span><span class="sxs-lookup"><span data-stu-id="67ed5-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="67ed5-114">R : les téléphones catégorisés en tant qu’appareils d’entreprise dans Intune ne sont pas identifiés avec leur numéro de téléphone complet lorsque, par exemple, vous exécutez un rapport sur l’inventaire des appareils mobiles.</span><span class="sxs-lookup"><span data-stu-id="67ed5-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="67ed5-115">Les numéros de téléphone des appareils sont toujours partiellement masqués par des astérisques (\*\*\*\*), et n'affichent que les quatre derniers chiffres.</span><span class="sxs-lookup"><span data-stu-id="67ed5-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>