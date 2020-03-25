---
title: Limitation de SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931440"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="93fa2-102">Limitation de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="93fa2-102">SharePoint Online throttling</span></span>

<span data-ttu-id="93fa2-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="93fa2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="93fa2-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="93fa2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="93fa2-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="93fa2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="93fa2-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="93fa2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="93fa2-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="93fa2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="93fa2-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="93fa2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="93fa2-109">**Limitation de SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="93fa2-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="93fa2-110">SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="93fa2-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="93fa2-111">Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources.</span><span class="sxs-lookup"><span data-stu-id="93fa2-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="93fa2-112">Pour plus d’informations, consultez les liens ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="93fa2-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="93fa2-113">Comment éviter d’être limité ou bloqué dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="93fa2-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="93fa2-114">Migration de données et limitation SPO</span><span class="sxs-lookup"><span data-stu-id="93fa2-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="93fa2-115">Vitesse de migration de SharePoint Online et OneDrive</span><span class="sxs-lookup"><span data-stu-id="93fa2-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="93fa2-116">Gérer la limitation de SharePoint Online à l’aide de la technique d’interruption exponentielle</span><span class="sxs-lookup"><span data-stu-id="93fa2-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="93fa2-117">Planification de la capacité et test de charge SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="93fa2-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

