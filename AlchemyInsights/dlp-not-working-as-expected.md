---
title: La DLP ne fonctionne pas comme prévu
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707808"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5e75f-102">La DLP ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="5e75f-102">DLP not working as expected</span></span>

<span data-ttu-id="5e75f-103">**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.</span><span class="sxs-lookup"><span data-stu-id="5e75f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="5e75f-104">**Configuration de la DLP**</span><span class="sxs-lookup"><span data-stu-id="5e75f-104">**Setting up DLP**</span></span>

<span data-ttu-id="5e75f-105">Avez-vous des problèmes avec la protection contre la perte de données **(DLP)** dans Office 365 qui ne fonctionne pas comme prévu ?</span><span class="sxs-lookup"><span data-stu-id="5e75f-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5e75f-106">Si c’est le cas, assurez-vous que votre stratégie **DLP** est correctement définie et que vos données contiennent ce que la stratégie **DLP** recherche lorsqu’elle est évaluée.</span><span class="sxs-lookup"><span data-stu-id="5e75f-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5e75f-107">Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="5e75f-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5e75f-108">Pour configurer des stratégies DLP, utilisez les informations [ici.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="5e75f-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="5e75f-109">**Ce que les stratégies DLP recherchent**</span><span class="sxs-lookup"><span data-stu-id="5e75f-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5e75f-110">Lors de l’utilisation des **types** d’informations sensibles intégrés dans les centres de sécurité et conformité, les stratégies DLP recherchent des modèles et des éléments spécifiques lors de la détection de ces types sensibles.</span><span class="sxs-lookup"><span data-stu-id="5e75f-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5e75f-111">**Types d’informations sensibles intégrés**</span><span class="sxs-lookup"><span data-stu-id="5e75f-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5e75f-112">Pour plus d’informations sur les types sensibles intégrés et ce qu’une stratégie DLP recherche lors de la détection du type sensible, voir : Ce que les types d’informations sensibles [recherchent.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5e75f-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="5e75f-113">**Types d’informations sensibles personnalisés**</span><span class="sxs-lookup"><span data-stu-id="5e75f-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5e75f-114">Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour plus d’informations sur la création d’un type d’informations sensibles personnalisé : Créer un [type d’informations sensibles personnalisé.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="5e75f-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5e75f-115">**Tester une stratégie DLP**</span><span class="sxs-lookup"><span data-stu-id="5e75f-115">**Test a DLP policy**</span></span>

<span data-ttu-id="5e75f-116">Pour tester vos données avec un type d’informations sensibles intégré ou personnalisé, utilisez l’option Type de **test** sous **Classifications** Types d’informations  >  **sensibles**.</span><span class="sxs-lookup"><span data-stu-id="5e75f-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5e75f-117">Pour plus d’informations, voir [Tester les types d’informations sensibles personnalisés.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="5e75f-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5e75f-118">**Rapports**</span><span class="sxs-lookup"><span data-stu-id="5e75f-118">**Reports**</span></span>
  
- <span data-ttu-id="5e75f-119">Obtenez des informations sur les données sensibles avec [les rapports DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="5e75f-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5e75f-120">Consultez les détails spécifiques de l’événement avec un [rapport d’incident.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="5e75f-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
