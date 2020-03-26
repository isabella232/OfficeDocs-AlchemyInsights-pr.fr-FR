---
title: Performances de la migration SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932002"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="f0221-102">Performances de la migration SharePoint</span><span class="sxs-lookup"><span data-stu-id="f0221-102">SharePoint migration performance</span></span>

<span data-ttu-id="f0221-103">**Important**: De nombreux clients SharePoint Online et OneDrive exécutent des applications critiques pour l’entreprise auprès du service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="f0221-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f0221-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="f0221-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f0221-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="f0221-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f0221-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="f0221-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f0221-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="f0221-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f0221-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="f0221-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f0221-109">**Performances de la migration**</span><span class="sxs-lookup"><span data-stu-id="f0221-109">**Migration performance**</span></span>

<span data-ttu-id="f0221-p103">Les performances de migration sont affectées par votre infrastructure réseau, la taille de fichier, l’heure de la migration et la limitation. Comprendre ceci vous permettra de planifier et optimiser l’efficacité de votre migration.</span><span class="sxs-lookup"><span data-stu-id="f0221-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="f0221-112">Pour plus d’informations, consultez les liens ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="f0221-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="f0221-113">Vitesse de migration de SharePoint Online et ODB</span><span class="sxs-lookup"><span data-stu-id="f0221-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="f0221-114">Comment éviter d’être limité ou bloqué dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f0221-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="f0221-115">Télécharger et installer l’Outil de migration SharePoint</span><span class="sxs-lookup"><span data-stu-id="f0221-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
