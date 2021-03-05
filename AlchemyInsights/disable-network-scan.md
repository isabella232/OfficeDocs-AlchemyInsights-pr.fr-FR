---
title: Désactiver l’analyse réseau
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449066"
---
# <a name="disable-network-scan"></a><span data-ttu-id="0f80d-102">Désactiver l’analyse réseau</span><span class="sxs-lookup"><span data-stu-id="0f80d-102">Disable network scan</span></span>

<span data-ttu-id="0f80d-103">Les analyses de partage réseau peuvent avoir un impact sur les performances.</span><span class="sxs-lookup"><span data-stu-id="0f80d-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="0f80d-104">Pour vous assurer que le client n’analyse pas les partages/fichiers réseau par défaut, configurez les paramètres suivants dans l’application Windows Defender sur **True**:</span><span class="sxs-lookup"><span data-stu-id="0f80d-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="0f80d-105">DisableScanningMappedNetworkDrivesForFullScan</span><span class="sxs-lookup"><span data-stu-id="0f80d-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="0f80d-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="0f80d-106">DisableScanningNetworkFiles</span></span>