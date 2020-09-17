---
title: Appareils Configuration Manager manquants dans le portail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812149"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="2a40e-102">Appareils Configuration Manager manquants dans le portail</span><span class="sxs-lookup"><span data-stu-id="2a40e-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="2a40e-103">Pour que la synchronisation des appareils fonctionne, des [points de terminaison Internet requis](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) doivent être accessibles à partir du serveur local qui héberge le rôle de point de connexion de service.</span><span class="sxs-lookup"><span data-stu-id="2a40e-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="2a40e-104">Pour résoudre les problèmes liés à la synchronisation des appareils, consultez le fichier **CMGatewaySyncUploadWorker.log** situé sur le point de connexion du service.</span><span class="sxs-lookup"><span data-stu-id="2a40e-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="2a40e-105">En savoir plus sur [la liaison client dans Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="2a40e-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
