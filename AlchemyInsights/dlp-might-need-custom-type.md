---
title: DLP peut avoir besoin d’un type personnalisé
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0ccdc524625ac76031004300a2406d5bfddcc759
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770315"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="81d76-102">DLP peut avoir besoin d’un type personnalisé</span><span class="sxs-lookup"><span data-stu-id="81d76-102">DLP might need a custom type</span></span>

<span data-ttu-id="81d76-103">Avec une stratégie de protection contre la perte de données (DLP), vous pouvez identifier et protéger les données sensibles de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="81d76-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="81d76-104">Dans certains cas, vous devrez peut-être créer votre \*\*\*\* propre type d’informations sensibles personnalisées pour protéger les données de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="81d76-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="81d76-105">Par exemple, votre organisation peut avoir besoin d’identifier et de protéger des ID d’employés ou d’autres données dans un format spécifique à votre organisation. Si c’est le cas, consultez les articles suivants pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="81d76-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="81d76-106">**Personnaliser un type d’informations sensibles intégré**</span><span class="sxs-lookup"><span data-stu-id="81d76-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="81d76-107">Si un type d’informations sensibles intégré répond à vos besoins avec seulement quelques ajustements, vous pouvez [personnaliser un type d’informations sensibles intégré](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="81d76-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="81d76-108">Par exemple, vous pouvez ajouter ou supprimer des mots clés, ou ajouter ou supprimer des preuves de prise en charge telles qu’une date ou une adresse.</span><span class="sxs-lookup"><span data-stu-id="81d76-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="81d76-109">**Créer un type d’informations sensibles personnalisé**</span><span class="sxs-lookup"><span data-stu-id="81d76-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="81d76-110">Toutefois, si vous devez identifier et protéger un autre type d’informations sensibles, vous pouvez [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) dans l’interface utilisateur du centre de sécurité & conformité.</span><span class="sxs-lookup"><span data-stu-id="81d76-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="81d76-111">**Créer un type d’informations sensibles personnalisé dans la sécurité & Centre de conformité PowerShell**</span><span class="sxs-lookup"><span data-stu-id="81d76-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="81d76-112">Enfin, si l’interface utilisateur ne fournit pas toutes les options dont vous avez besoin, vous pouvez [créer un type d’informations sensibles personnalisé dans la sécurité & Centre de conformité PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="81d76-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="81d76-113">En commençant par un fichier XML, vous pouvez utiliser toutes les options disponibles.</span><span class="sxs-lookup"><span data-stu-id="81d76-113">By starting with an XML file, you can use every option available.</span></span>

    
