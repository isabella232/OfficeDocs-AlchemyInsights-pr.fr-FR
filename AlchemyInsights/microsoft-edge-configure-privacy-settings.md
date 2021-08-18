---
title: Microsoft Edge configurer les paramètres de confidentialité
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114170"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurer les paramètres de confidentialité

Par défaut, si Microsoft Edge est déployé sur des plateformes non Windows, les données de diagnostic et les informations de site ne sont pas envoyées à Microsoft. Toutefois, si Microsoft Edge est déployé sur Windows 10, les données de diagnostic et les informations de site sont envoyées conformément aux paramètres de données de diagnostic Windows [utilisateurs.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Pour configurer la façon dont Microsoft Edge collecte de données pour votre organisation, utilisez les stratégies de groupe suivantes :
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): cette stratégie permet de signaler les données d’utilisation et d’incident.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): cette stratégie envoie des informations de site qui sont utilisées pour améliorer services Microsoft.

Pour plus d’informations, voir [Configurer les paramètres de stratégie.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)