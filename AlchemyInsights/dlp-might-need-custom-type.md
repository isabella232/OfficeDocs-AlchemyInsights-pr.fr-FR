---
title: DLP peut avoir besoin d’un type personnalisé
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932656"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="3fcc4-102">DLP peut avoir besoin d’un type personnalisé</span><span class="sxs-lookup"><span data-stu-id="3fcc4-102">DLP might need a custom type</span></span>

<span data-ttu-id="3fcc4-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3fcc4-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3fcc4-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3fcc4-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3fcc4-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3fcc4-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3fcc4-109">**DLP peut nécessiter un type d’informations personnalisé**</span><span class="sxs-lookup"><span data-stu-id="3fcc4-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="3fcc4-110">Avec une stratégie de protection contre la perte de données (DLP), vous pouvez identifier et protéger les données sensibles de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="3fcc4-111">Dans certains cas, vous devrez peut-être créer votre propre type d’informations sensibles **personnalisées** pour protéger les données de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="3fcc4-112">Par exemple, votre organisation peut avoir besoin d’identifier et de protéger des ID d’employés ou d’autres données dans un format spécifique à votre organisation. Si c’est le cas, consultez les articles suivants pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="3fcc4-113">**Personnaliser un type d’informations sensibles intégré**</span><span class="sxs-lookup"><span data-stu-id="3fcc4-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="3fcc4-114">Si un type d’informations sensibles intégré répond à vos besoins avec seulement quelques ajustements, vous pouvez [personnaliser un type d’informations sensibles intégré](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3fcc4-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="3fcc4-115">Par exemple, vous pouvez ajouter ou supprimer des mots clés, ou ajouter ou supprimer des preuves de prise en charge telles qu’une date ou une adresse.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="3fcc4-116">**Créer un type d’informations sensibles personnalisé**</span><span class="sxs-lookup"><span data-stu-id="3fcc4-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="3fcc4-117">Toutefois, si vous devez identifier et protéger un autre type d’informations sensibles, vous pouvez [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) dans l’interface utilisateur du centre de sécurité & conformité.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="3fcc4-118">**Créer un type d’informations sensibles personnalisé dans l’interface PowerShell du Centre de sécurité et conformité**</span><span class="sxs-lookup"><span data-stu-id="3fcc4-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="3fcc4-119">Enfin, si l’interface utilisateur ne fournit pas toutes les options dont vous avez besoin, vous pouvez [créer un type d’informations sensibles personnalisé dans la sécurité & Centre de conformité PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="3fcc4-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="3fcc4-120">En commençant par un fichier XML, vous pouvez utiliser toutes les options disponibles.</span><span class="sxs-lookup"><span data-stu-id="3fcc4-120">By starting with an XML file, you can use every option available.</span></span>
