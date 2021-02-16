---
title: Activer l’appareil
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255159"
---
# <a name="enable-device"></a><span data-ttu-id="109de-102">Activer l’appareil</span><span class="sxs-lookup"><span data-stu-id="109de-102">Enable Device</span></span>

<span data-ttu-id="109de-103">**Pour activer l’appareil à l’aide de la commande PowerShell**</span><span class="sxs-lookup"><span data-stu-id="109de-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="109de-104">Exécutez les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="109de-104">Run the following commands:</span></span>

- <span data-ttu-id="109de-105">Pour obtenir l’objet appareil : `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="109de-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="109de-106">Pour activer l’appareil : `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="109de-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="109de-107">Pour plus d’informations sur la configuration de la jointage hybride sur les domaines gérés, voir [Configurer la jointage hybride.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)</span><span class="sxs-lookup"><span data-stu-id="109de-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
