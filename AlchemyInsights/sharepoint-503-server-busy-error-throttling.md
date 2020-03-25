---
title: Limitation de SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931224"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="ee316-102">Limitation de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ee316-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="ee316-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="ee316-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ee316-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="ee316-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ee316-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="ee316-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ee316-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="ee316-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ee316-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="ee316-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ee316-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="ee316-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ee316-109">**erreur de disponibilité du serveur 503**</span><span class="sxs-lookup"><span data-stu-id="ee316-109">**503 server is busy error**</span></span>

<span data-ttu-id="ee316-110">Les utilisateurs peuvent recevoir un message d’erreur « le serveur 503 est occupé » lors de la tentative de navigation vers des sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ee316-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="ee316-111">Cette erreur peut être causée par la limitation dans le service SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ee316-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ee316-112">SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ee316-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ee316-113">Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources.</span><span class="sxs-lookup"><span data-stu-id="ee316-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="ee316-114">Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ee316-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="ee316-115">Si vous pensez que cette erreur n’est pas liée à la limitation, vous pouvez vérifier si la maintenance active a lieu sur votre client en accédant au [Centre de messages](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="ee316-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="ee316-116">Enfin, vous devez consulter la page [État du service](https://portal.office.com/adminportal/home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire.</span><span class="sxs-lookup"><span data-stu-id="ee316-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

