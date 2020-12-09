---
title: Paramètres de confidentialité de la configuration de Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599477"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Paramètres de confidentialité de la configuration de Microsoft Edge

Par défaut, si Microsoft Edge est déployé sur des plateformes autres que Windows, les données de diagnostic et les informations de site ne sont pas envoyées à Microsoft. Toutefois, si Microsoft Edge est déployé sur Windows 10, les données de diagnostic et les informations de site sont envoyées conformément aux [paramètres des données de diagnostic Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)de l’utilisateur.

Pour configurer la façon dont Microsoft Edge gère la collecte de données pour votre organisation, utilisez les stratégies de groupe suivantes :
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): cette stratégie active la création de rapports sur les données relatives à l’utilisation et aux incidents.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): cette stratégie envoie les informations de site utilisées pour améliorer les services Microsoft.

Pour plus d’informations, consultez la rubrique [configurer les paramètres de stratégie](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).