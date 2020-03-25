---
title: Plus d’informations sur les problèmes liés à DLP
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932692"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="5160d-102">Informations sur les problèmes liés à DLP</span><span class="sxs-lookup"><span data-stu-id="5160d-102">Information about DLP issues</span></span>

<span data-ttu-id="5160d-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="5160d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5160d-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="5160d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5160d-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="5160d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5160d-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="5160d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5160d-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="5160d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5160d-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="5160d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5160d-109">**Informations sur la stratégie DLP**</span><span class="sxs-lookup"><span data-stu-id="5160d-109">**Information on DLP policy**</span></span>

<span data-ttu-id="5160d-110">Avec une stratégie DLP, vous pouvez identifier, surveiller et protéger automatiquement les informations sensibles dans Office 365.</span><span class="sxs-lookup"><span data-stu-id="5160d-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="5160d-111">Pour plus d’informations, consultez les liens suivants :</span><span class="sxs-lookup"><span data-stu-id="5160d-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="5160d-112">Vue d’ensemble de la protection contre la perte de données</span><span class="sxs-lookup"><span data-stu-id="5160d-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="5160d-113">Éléments recherchés par les types d’informations sensibles</span><span class="sxs-lookup"><span data-stu-id="5160d-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="5160d-114">Créer un type d’informations sensibles personnalisé</span><span class="sxs-lookup"><span data-stu-id="5160d-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="5160d-115">Envoyer des notifications par courrier électronique et afficher des conseils de stratégie</span><span class="sxs-lookup"><span data-stu-id="5160d-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="5160d-116">Protéger les fichiers SharePoint Online avec des étiquettes de rétention et la protection contre la perte de données (DLP)</span><span class="sxs-lookup"><span data-stu-id="5160d-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="5160d-117">DLP et Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5160d-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="5160d-118">Pour tester vos données à l’aide d’un type d’informations sensibles intégré ou personnalisé, utilisez l’option **type de test** sous types d’informations**sensibles**sur les **classifications** > .</span><span class="sxs-lookup"><span data-stu-id="5160d-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5160d-119">Pour plus d’informations, consultez la rubrique [test des types d’informations sensibles personnalisés](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="5160d-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>