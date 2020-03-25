---
title: DLP ne fonctionne pas comme prévu
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932620"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c2812-102">DLP ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="c2812-102">DLP not working as expected</span></span>

<span data-ttu-id="c2812-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="c2812-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c2812-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="c2812-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c2812-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="c2812-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c2812-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="c2812-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c2812-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="c2812-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c2812-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="c2812-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="c2812-109">**Configuration de DLP**</span><span class="sxs-lookup"><span data-stu-id="c2812-109">**Setting up DLP**</span></span>

<span data-ttu-id="c2812-110">Rencontrez-vous des problèmes avec la **protection contre la perte de données (DLP)** dans Office 365 ne fonctionnent pas comme prévu ?</span><span class="sxs-lookup"><span data-stu-id="c2812-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c2812-111">Si c’est le cas, assurez-vous que votre **stratégie DLP** est correctement configurée et que vos données contiennent ce que la **stratégie DLP** recherche lors de l’évaluation.</span><span class="sxs-lookup"><span data-stu-id="c2812-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="c2812-112">Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c2812-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c2812-113">Pour configurer les stratégies DLP, utilisez les informations [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="c2812-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="c2812-114">**Stratégies DLP**</span><span class="sxs-lookup"><span data-stu-id="c2812-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="c2812-115">Lors de l’utilisation des **types d’informations sensibles intégrés** dans le centre de sécurité et de conformité Office 365, les stratégies DLP recherchent des éléments et des modèles spécifiques lors de la détection de ces types sensibles.</span><span class="sxs-lookup"><span data-stu-id="c2812-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="c2812-116">**Types d’informations sensibles intégrés**</span><span class="sxs-lookup"><span data-stu-id="c2812-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="c2812-117">Pour plus d’informations sur les types sensibles intégrés et sur ce qu’une stratégie DLP doit rechercher lors de la détection du type sensible, voir : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="c2812-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="c2812-118">**Types d’informations sensibles personnalisés**</span><span class="sxs-lookup"><span data-stu-id="c2812-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="c2812-119">Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour obtenir des informations sur la création d’un type de données sensibles personnalisé : [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c2812-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="c2812-120">**Tester une stratégie DLP**</span><span class="sxs-lookup"><span data-stu-id="c2812-120">**Test a DLP policy**</span></span>

<span data-ttu-id="c2812-121">Pour tester vos données à l’aide d’un type d’informations sensibles intégré ou personnalisé, utilisez l’option **type de test** sous types d’informations**sensibles**sur les **classifications** > .</span><span class="sxs-lookup"><span data-stu-id="c2812-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="c2812-122">Pour plus d’informations, consultez la rubrique [test des types d’informations sensibles personnalisés](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="c2812-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="c2812-123">**Rapports**</span><span class="sxs-lookup"><span data-stu-id="c2812-123">**Reports**</span></span>
  
- <span data-ttu-id="c2812-124">Obtenez des données sensibles à l’aide des [rapports DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c2812-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="c2812-125">Consultez les détails spécifiques de l’événement à l’aide d’un [rapport d’incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="c2812-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
