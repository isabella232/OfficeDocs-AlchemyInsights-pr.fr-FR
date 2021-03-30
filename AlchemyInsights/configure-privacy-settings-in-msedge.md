---
title: Configurer les paramètres de confidentialité dans Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403815"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Configurer les paramètres de confidentialité dans Microsoft Edge

Par défaut, si Microsoft Edge est déployé sur des plateformes autres que Windows, les données de diagnostic et les informations de site ne sont pas envoyées à Microsoft. Toutefois, si Microsoft Edge est déployé sur Windows 10, les données de diagnostic et les informations de site sont envoyées en fonction des paramètres de données de [diagnostic Windows des utilisateurs.](https://go.microsoft.com/fwlink/?linkid=2132472)

Pour configurer la façon dont Microsoft Edge gère la collecte de données pour votre organisation, utilisez les stratégies de groupe suivantes :
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) permet de signaler les données relatives à l’utilisation et aux incidents.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) envoie des informations de site utilisées pour améliorer les services Microsoft.

Pour plus d’informations, voir [Configurer les paramètres de stratégie.](https://go.microsoft.com/fwlink/?linkid=2132577)
