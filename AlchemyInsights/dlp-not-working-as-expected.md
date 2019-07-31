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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941066"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="04e5d-102">DLP ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="04e5d-102">DLP not working as expected</span></span>

<span data-ttu-id="04e5d-103">Rencontrez-vous des problèmes avec la **protection contre la perte de données (DLP)** dans Office 365 ne fonctionnent pas comme prévu?</span><span class="sxs-lookup"><span data-stu-id="04e5d-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="04e5d-104">Si c’est le cas, assurez-vous que votre **stratégie DLP** est correctement configurée et que vos données contiennent ce que la **stratégie DLP** recherche lors de l’évaluation.</span><span class="sxs-lookup"><span data-stu-id="04e5d-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="04e5d-105">**Configuration de DLP**</span><span class="sxs-lookup"><span data-stu-id="04e5d-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="04e5d-106">Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="04e5d-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="04e5d-107">Pour configurer les stratégies DLP, utilisez les informations [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="04e5d-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="04e5d-108">**Stratégies DLP**</span><span class="sxs-lookup"><span data-stu-id="04e5d-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="04e5d-109">Lors de l’utilisation des **types d’informations sensibles intégrés** dans le centre de sécurité et de conformité Office 365, les stratégies DLP recherchent des éléments et des modèles spécifiques lors de la détection de ces types sensibles.</span><span class="sxs-lookup"><span data-stu-id="04e5d-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="04e5d-110">**Types d’informations sensibles intégrés**</span><span class="sxs-lookup"><span data-stu-id="04e5d-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="04e5d-111">Pour plus d’informations sur les types sensibles intégrés et sur ce qu’une stratégie DLP doit rechercher lors de la détection du type sensible, voir: [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="04e5d-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="04e5d-112">**Types d’informations sensibles personnalisés**</span><span class="sxs-lookup"><span data-stu-id="04e5d-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="04e5d-113">Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour obtenir des informations sur la création d’un type de données sensibles personnalisé: [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="04e5d-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="04e5d-114">**Tester une stratégie DLP**</span><span class="sxs-lookup"><span data-stu-id="04e5d-114">**Test a DLP policy**</span></span>

<span data-ttu-id="04e5d-115">Pour tester vos données à l’aide d’un type d’informations sensibles intégré ou personnalisé, utilisez l’option **type de test** sous types d’informations**sensibles**sur les **classifications** > .</span><span class="sxs-lookup"><span data-stu-id="04e5d-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="04e5d-116">Pour plus d’informations, consultez la rubrique [test des types d’informations sensibles personnalisés](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="04e5d-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="04e5d-117">**Rapports**</span><span class="sxs-lookup"><span data-stu-id="04e5d-117">**Reports**</span></span>
  
- <span data-ttu-id="04e5d-118">Obtenez des données sensibles à l’aide des [rapports DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="04e5d-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="04e5d-119">Consultez les détails spécifiques de l’événement à l’aide d’un [rapport d’incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="04e5d-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
