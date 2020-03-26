---
title: Conseils généraux en matière de performances de migration
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932477"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="3a88c-102">Conseils généraux en matière de performances de migration</span><span class="sxs-lookup"><span data-stu-id="3a88c-102">General migration performance guidance</span></span>

<span data-ttu-id="3a88c-103">**Important**: De nombreux clients SharePoint Online et OneDrive exécutent des applications critiques pour l’entreprise auprès du service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="3a88c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3a88c-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="3a88c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3a88c-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="3a88c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3a88c-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="3a88c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3a88c-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="3a88c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3a88c-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="3a88c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3a88c-109">**Conseils sur les performances de migration**</span><span class="sxs-lookup"><span data-stu-id="3a88c-109">**Migration performance guidance**</span></span>

<span data-ttu-id="3a88c-p103">Les performances de migration sont affectées par votre infrastructure réseau, la taille de fichier, l’heure de la migration et la limitation. Comprendre ceci vous permettra de planifier et optimiser l’efficacité de votre migration.</span><span class="sxs-lookup"><span data-stu-id="3a88c-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="3a88c-112">Conseils généraux relatifs aux performances de migration</span><span class="sxs-lookup"><span data-stu-id="3a88c-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
