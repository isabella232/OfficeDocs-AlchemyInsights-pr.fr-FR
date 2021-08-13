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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966107"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Appareils Configuration Manager manquants dans le portail

Pour que la synchronisation des appareils fonctionne, des [points de terminaison Internet requis](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) doivent être accessibles à partir du serveur local qui héberge le rôle de point de connexion de service. Pour résoudre les problèmes liés à la synchronisation des appareils, consultez le fichier **CMGatewaySyncUploadWorker.log** situé sur le point de connexion du service.

En savoir plus sur [la liaison client dans Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
