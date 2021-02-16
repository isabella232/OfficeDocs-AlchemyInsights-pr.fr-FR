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
# <a name="enable-device"></a>Activer l’appareil

**Pour activer l’appareil à l’aide de la commande PowerShell**

Exécutez les commandes suivantes :

- Pour obtenir l’objet appareil : `Get-MsolDevice -Name <Name>`
- Pour activer l’appareil : `Enable-MsolDevice -DeviceId <DeviceId>`

Pour plus d’informations sur la configuration de la jointage hybride sur les domaines gérés, voir [Configurer la jointage hybride.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
