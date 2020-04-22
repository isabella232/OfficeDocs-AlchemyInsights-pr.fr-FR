---
title: DLP peut avoir besoin d’un type personnalisé
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704487"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="c10fc-102">DLP peut avoir besoin d’un type personnalisé</span><span class="sxs-lookup"><span data-stu-id="c10fc-102">DLP might need a custom type</span></span>

<span data-ttu-id="c10fc-103">**Important**: En ces temps sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint en ligne et OneDrive demeurent très disponibles – Veuillez consulter [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.</span><span class="sxs-lookup"><span data-stu-id="c10fc-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c10fc-104">**DLP peut nécessiter un type d’informations personnalisé**</span><span class="sxs-lookup"><span data-stu-id="c10fc-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="c10fc-105">Avec une stratégie de protection contre la perte de données (DLP), vous pouvez identifier et protéger les données sensibles de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c10fc-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="c10fc-106">Dans certains cas, vous devrez peut-être créer votre propre type d’informations sensibles **personnalisées** pour protéger les données de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c10fc-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="c10fc-107">Par exemple, votre organisation peut avoir besoin d’identifier et de protéger des ID d’employés ou d’autres données dans un format spécifique à votre organisation. Si c’est le cas, consultez les articles suivants pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="c10fc-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="c10fc-108">**Personnaliser un type d’informations sensibles intégré**</span><span class="sxs-lookup"><span data-stu-id="c10fc-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="c10fc-109">Si un type d’informations sensibles intégré répond à vos besoins avec seulement quelques ajustements, vous pouvez [personnaliser un type d’informations sensibles intégré](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c10fc-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="c10fc-110">Par exemple, vous pouvez ajouter ou supprimer des mots clés, ou ajouter ou supprimer des preuves de prise en charge telles qu’une date ou une adresse.</span><span class="sxs-lookup"><span data-stu-id="c10fc-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="c10fc-111">**Créer un type d’informations sensibles personnalisé**</span><span class="sxs-lookup"><span data-stu-id="c10fc-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="c10fc-112">Toutefois, si vous devez identifier et protéger un autre type d’informations sensibles, vous pouvez [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) dans l’interface utilisateur du centre de sécurité & conformité.</span><span class="sxs-lookup"><span data-stu-id="c10fc-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="c10fc-113">**Créer un type d’informations sensibles personnalisé dans l’interface PowerShell du Centre de sécurité et conformité**</span><span class="sxs-lookup"><span data-stu-id="c10fc-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="c10fc-114">Enfin, si l’interface utilisateur ne fournit pas toutes les options dont vous avez besoin, vous pouvez [créer un type d’informations sensibles personnalisé dans la sécurité & Centre de conformité PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="c10fc-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="c10fc-115">En commençant par un fichier XML, vous pouvez utiliser toutes les options disponibles.</span><span class="sxs-lookup"><span data-stu-id="c10fc-115">By starting with an XML file, you can use every option available.</span></span>
