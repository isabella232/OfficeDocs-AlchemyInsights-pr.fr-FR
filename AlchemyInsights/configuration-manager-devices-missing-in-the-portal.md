---
title: Appareils Configuration Manager manquants dans le portail
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817242"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="55a65-102">Appareils Configuration Manager manquants dans le portail</span><span class="sxs-lookup"><span data-stu-id="55a65-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="55a65-103">Pour que la synchronisation des appareils fonctionne, des [points de terminaison Internet requis](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) doivent être accessibles à partir du serveur local qui héberge le rôle de point de connexion de service.</span><span class="sxs-lookup"><span data-stu-id="55a65-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="55a65-104">Pour résoudre les problèmes liés à la synchronisation des appareils, consultez le fichier **CMGatewaySyncUploadWorker.log** situé sur le point de connexion du service.</span><span class="sxs-lookup"><span data-stu-id="55a65-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="55a65-105">En savoir plus sur [la liaison client dans Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="55a65-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
