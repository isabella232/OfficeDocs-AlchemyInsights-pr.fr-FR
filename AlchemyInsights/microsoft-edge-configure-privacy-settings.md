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
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="84c8d-102">Paramètres de confidentialité de la configuration de Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="84c8d-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="84c8d-103">Par défaut, si Microsoft Edge est déployé sur des plateformes autres que Windows, les données de diagnostic et les informations de site ne sont pas envoyées à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="84c8d-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="84c8d-104">Toutefois, si Microsoft Edge est déployé sur Windows 10, les données de diagnostic et les informations de site sont envoyées conformément aux [paramètres des données de diagnostic Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="84c8d-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="84c8d-105">Pour configurer la façon dont Microsoft Edge gère la collecte de données pour votre organisation, utilisez les stratégies de groupe suivantes :</span><span class="sxs-lookup"><span data-stu-id="84c8d-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="84c8d-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): cette stratégie active la création de rapports sur les données relatives à l’utilisation et aux incidents.</span><span class="sxs-lookup"><span data-stu-id="84c8d-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="84c8d-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): cette stratégie envoie les informations de site utilisées pour améliorer les services Microsoft.</span><span class="sxs-lookup"><span data-stu-id="84c8d-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="84c8d-108">Pour plus d’informations, consultez la rubrique [configurer les paramètres de stratégie](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="84c8d-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>