---
title: Dépannage des erreurs et problèmes liés à l’outil de migration SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931116"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="789ea-102">Dépannage des erreurs et problèmes liés à l’outil de migration SharePoint</span><span class="sxs-lookup"><span data-stu-id="789ea-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="789ea-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="789ea-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="789ea-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="789ea-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="789ea-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="789ea-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="789ea-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="789ea-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="789ea-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="789ea-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="789ea-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="789ea-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="789ea-109">**Problèmes courants et Erreurs**</span><span class="sxs-lookup"><span data-stu-id="789ea-109">**Common issues and errors**</span></span>

<span data-ttu-id="789ea-110">Vous pouvez rencontrer des problèmes et des erreurs courants lors de l’utilisation de l’outil de migration SharePoint (SPMT).</span><span class="sxs-lookup"><span data-stu-id="789ea-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="789ea-111">Pour plus d’informations, consultez les liens ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="789ea-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="789ea-112">Résolution des erreurs et des problèmes SPMT courants</span><span class="sxs-lookup"><span data-stu-id="789ea-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="789ea-113">Résolution des problèmes d’installation de SPMT</span><span class="sxs-lookup"><span data-stu-id="789ea-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)