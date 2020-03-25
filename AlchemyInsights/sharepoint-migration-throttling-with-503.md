---
title: Limitation de la migration SharePoint avec 503 Erreurs
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931656"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="91ac1-102">Limitation de la migration SharePoint avec 503 Erreurs</span><span class="sxs-lookup"><span data-stu-id="91ac1-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="91ac1-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="91ac1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="91ac1-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="91ac1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="91ac1-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="91ac1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="91ac1-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="91ac1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="91ac1-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="91ac1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="91ac1-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="91ac1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="91ac1-109">**503 Erreurs lors de la migration vers SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="91ac1-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="91ac1-110">Il s’avère que vous effectuez une migration vers SharePoint Online et que vous recevez des erreurs 503.</span><span class="sxs-lookup"><span data-stu-id="91ac1-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="91ac1-111">Suivez les étapes ci-dessous pour que nous puissions vous aider dès que possible.</span><span class="sxs-lookup"><span data-stu-id="91ac1-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="91ac1-112">Cliquez sur **contacter le support**, puis sur **nouvelle demande de service**.</span><span class="sxs-lookup"><span data-stu-id="91ac1-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="91ac1-113">Pour le titre et la description, tapez **limitation de migration SharePoint avec 503**.</span><span class="sxs-lookup"><span data-stu-id="91ac1-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="91ac1-114">Une fois le ticket soumis, veuillez le mettre à jour avec les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="91ac1-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="91ac1-115">La quantité de migration (par exemple, le nombre de TBs ?).</span><span class="sxs-lookup"><span data-stu-id="91ac1-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="91ac1-116">Date de début et de fin de la migration.</span><span class="sxs-lookup"><span data-stu-id="91ac1-116">Migration start and end date.</span></span>
    - <span data-ttu-id="91ac1-117">Décrivez l’emplacement à partir duquel vous migrez votre contenu (par exemple, SharePoint Server, Box, GDrive, partages de fichiers, etc.).</span><span class="sxs-lookup"><span data-stu-id="91ac1-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="91ac1-118">Estimez le nombre d’erreurs de limitation (par exemple, la limitation x par heure ?) et la durée de la limitation.</span><span class="sxs-lookup"><span data-stu-id="91ac1-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="91ac1-119">L’outil de migration que vous utilisez (par exemple, SPMT ou ShareGate).</span><span class="sxs-lookup"><span data-stu-id="91ac1-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


