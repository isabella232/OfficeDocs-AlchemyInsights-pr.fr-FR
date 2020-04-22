---
title: DLP ne fonctionne pas comme prévu
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704411"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="34c56-102">DLP ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="34c56-102">DLP not working as expected</span></span>

<span data-ttu-id="34c56-103">**Important**: En ces temps sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint en ligne et OneDrive demeurent très disponibles – Veuillez consulter [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.</span><span class="sxs-lookup"><span data-stu-id="34c56-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="34c56-104">**Configuration de DLP**</span><span class="sxs-lookup"><span data-stu-id="34c56-104">**Setting up DLP**</span></span>

<span data-ttu-id="34c56-105">Rencontrez-vous des problèmes avec la **protection contre la perte de données (DLP)** dans Office 365 ne fonctionnent pas comme prévu ?</span><span class="sxs-lookup"><span data-stu-id="34c56-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="34c56-106">Si c’est le cas, assurez-vous que votre **stratégie DLP** est correctement configurée et que vos données contiennent ce que la **stratégie DLP** recherche lors de l’évaluation.</span><span class="sxs-lookup"><span data-stu-id="34c56-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="34c56-107">Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="34c56-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="34c56-108">Pour configurer les stratégies DLP, utilisez les informations [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="34c56-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="34c56-109">**Stratégies DLP**</span><span class="sxs-lookup"><span data-stu-id="34c56-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="34c56-110">Lors de l’utilisation des **types d’informations sensibles intégrés** dans les centres de sécurité et de conformité, les stratégies DLP recherchent des éléments et des modèles spécifiques lors de la détection de ces types sensibles.</span><span class="sxs-lookup"><span data-stu-id="34c56-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="34c56-111">**Types d’informations sensibles intégrés**</span><span class="sxs-lookup"><span data-stu-id="34c56-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="34c56-112">Pour plus d’informations sur les types sensibles intégrés et sur ce qu’une stratégie DLP doit rechercher lors de la détection du type sensible, voir : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="34c56-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="34c56-113">**Types d’informations sensibles personnalisés**</span><span class="sxs-lookup"><span data-stu-id="34c56-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="34c56-114">Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour obtenir des informations sur la création d’un type de données sensibles personnalisé : [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="34c56-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="34c56-115">**Tester une stratégie DLP**</span><span class="sxs-lookup"><span data-stu-id="34c56-115">**Test a DLP policy**</span></span>

<span data-ttu-id="34c56-116">Pour tester vos données à l’aide d’un type d’informations sensibles intégré ou personnalisé, utilisez l’option **type de test** sous types d’informations**sensibles**sur les **classifications** > .</span><span class="sxs-lookup"><span data-stu-id="34c56-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="34c56-117">Pour plus d’informations, consultez la rubrique [test des types d’informations sensibles personnalisés](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="34c56-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="34c56-118">**Rapports**</span><span class="sxs-lookup"><span data-stu-id="34c56-118">**Reports**</span></span>
  
- <span data-ttu-id="34c56-119">Obtenez des données sensibles à l’aide des [rapports DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="34c56-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="34c56-120">Consultez les détails spécifiques de l’événement à l’aide d’un [rapport d’incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="34c56-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
