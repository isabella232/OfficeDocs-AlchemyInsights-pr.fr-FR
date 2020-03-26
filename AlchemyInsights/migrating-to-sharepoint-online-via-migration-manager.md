---
title: Migration vers SharePoint Online via le Gestionnaire de migration
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931974"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="39edb-102">Migration vers SharePoint Online via le Gestionnaire de migration</span><span class="sxs-lookup"><span data-stu-id="39edb-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="39edb-103">**Important**: De nombreux clients SharePoint Online et OneDrive exécutent des applications critiques pour l’entreprise auprès du service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="39edb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="39edb-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="39edb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="39edb-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="39edb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="39edb-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="39edb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="39edb-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="39edb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="39edb-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="39edb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="39edb-109">**Gestionnaire de migration**</span><span class="sxs-lookup"><span data-stu-id="39edb-109">**Migration Manager**</span></span>

<span data-ttu-id="39edb-110">Situé dans le Centre d’administration SharePoint moderne, le Gestionnaire de migration vous guide dans la configuration de vos clients et la création de vos tâches.</span><span class="sxs-lookup"><span data-stu-id="39edb-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="39edb-111">Vous pouvez spécifier des paramètres globaux ou de niveau tâche, afficher l’état d’avancement de toutes les tâches et télécharger des rapports sommaires agrégés et de niveau tâche.</span><span class="sxs-lookup"><span data-stu-id="39edb-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="39edb-112">Prise en main du Gestionnaire de migration</span><span class="sxs-lookup"><span data-stu-id="39edb-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="39edb-113">Configurer les clients du Gestionnaire de migration</span><span class="sxs-lookup"><span data-stu-id="39edb-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="39edb-114">Paramètres du Gestionnaire de migration</span><span class="sxs-lookup"><span data-stu-id="39edb-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
