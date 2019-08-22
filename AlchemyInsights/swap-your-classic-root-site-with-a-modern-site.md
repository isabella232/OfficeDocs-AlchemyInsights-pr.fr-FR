---
title: Échangez votre site racine classique avec un site moderne
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501077"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="fc049-102">Échangez votre site racine classique avec un site moderne</span><span class="sxs-lookup"><span data-stu-id="fc049-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="fc049-103">Si votre environnement a été configuré avant le 2019 avril, vous pouvez remplacer votre site racine par un site moderne à l’aide de Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="fc049-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="fc049-104">Si vous souhaitez utiliser un autre site que celui de votre site racine, vous pouvez remplacer (remplacer) le site racine par celui-ci.</span><span class="sxs-lookup"><span data-stu-id="fc049-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="fc049-105">Utilisez [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site sur un autre site lors de l’archivage du site d’origine.</span><span class="sxs-lookup"><span data-stu-id="fc049-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="fc049-106">Disponible pour les deux sites d’équipe (non connecté à un groupe) et le site de communication.</span><span class="sxs-lookup"><span data-stu-id="fc049-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="fc049-107">Des fonctionnalités supplémentaires seront bientôt introduites, qui vous permettront de continuer à utiliser le contenu sur le site, mais convertissez le site existant en un site de communication.</span><span class="sxs-lookup"><span data-stu-id="fc049-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="fc049-108">Ces fonctionnalités seront déployées graduellement.</span><span class="sxs-lookup"><span data-stu-id="fc049-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="fc049-109">Continuez à consulter le centre de messages Office 365 pour les mises à jour.</span><span class="sxs-lookup"><span data-stu-id="fc049-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="fc049-110">Problèmes connus liés à l’échange de sites</span><span class="sxs-lookup"><span data-stu-id="fc049-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="fc049-111">Le site cible peut renvoyer une erreur «introuvable» (HTTP 404) pendant une courte période de temps.</span><span class="sxs-lookup"><span data-stu-id="fc049-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="fc049-112">Le contenu doit être réanalysé pour mettre à jour l’index de recherche.</span><span class="sxs-lookup"><span data-stu-id="fc049-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="fc049-113">Aucune étape manuelle n’est requise: cette opération sera automatique.</span><span class="sxs-lookup"><span data-stu-id="fc049-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="fc049-114">Tout ce qui dépend de liens «statiques» (tels que la synchronisation de fichiers et les fichiers OneNote) doit être corrigé manuellement.</span><span class="sxs-lookup"><span data-stu-id="fc049-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="fc049-115">Si le site source était un site de News de l’organisation, mettez à jour l’URL.</span><span class="sxs-lookup"><span data-stu-id="fc049-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="fc049-116">Obtenir la liste de tous les sites d’actualité de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="fc049-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="fc049-117">Les sites Project Server peuvent avoir besoin d’être validés pour s’assurer qu’ils sont toujours correctement associés.</span><span class="sxs-lookup"><span data-stu-id="fc049-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





