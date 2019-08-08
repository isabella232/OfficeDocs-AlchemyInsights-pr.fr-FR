---
title: Site moderne comme site racine
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232713"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="a6796-102">Site moderne en tant que site racine</span><span class="sxs-lookup"><span data-stu-id="a6796-102">Modern site as root site</span></span>

<span data-ttu-id="a6796-103">Nous avons commencé à déployer une nouvelle fonctionnalité qui vous permettra d’échanger votre site racine de site classique à l’aide d’un site moderne.</span><span class="sxs-lookup"><span data-stu-id="a6796-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="a6796-104">Utilisez [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site sur un autre site lors de l’archivage du site d’origine.</span><span class="sxs-lookup"><span data-stu-id="a6796-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="a6796-105">Disponible pour les deux sites d’équipe (non connecté à un groupe) et le site de communication.</span><span class="sxs-lookup"><span data-stu-id="a6796-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="a6796-106">Ne supprimez pas votre site racine classique pour créer un site de communication moderne.</span><span class="sxs-lookup"><span data-stu-id="a6796-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="a6796-107">Ceci n’est pas pris en charge par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a6796-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="a6796-108">La suppression du site racine rendra tous les sites SharePoint de votre organisation inaccessibles à tous les utilisateurs, jusqu’à ce que vous restauriez le site ou que vous créez un nouveau site à la même URL.</span><span class="sxs-lookup"><span data-stu-id="a6796-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="a6796-109">Nous communiquerons cette fonctionnalité via le centre de messages.</span><span class="sxs-lookup"><span data-stu-id="a6796-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="a6796-110">Attendez-vous à ce que la fonctionnalité soit activée dans votre client.</span><span class="sxs-lookup"><span data-stu-id="a6796-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="a6796-111">Problèmes connus liés à l’échange de sites</span><span class="sxs-lookup"><span data-stu-id="a6796-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="a6796-112">Le site cible peut renvoyer une erreur «introuvable» (HTTP 404) pendant une courte période de temps.</span><span class="sxs-lookup"><span data-stu-id="a6796-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="a6796-113">Le contenu doit être réanalysé pour mettre à jour l’index de recherche.</span><span class="sxs-lookup"><span data-stu-id="a6796-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="a6796-114">Il n’y a pas d’étape manuelle requise ici, cette opération sera exécutée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="a6796-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="a6796-115">Tout ce qui dépend de liens «statiques» (tels que la synchronisation de fichiers et les fichiers OneNote) doit être corrigé manuellement.</span><span class="sxs-lookup"><span data-stu-id="a6796-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="a6796-116">Les sites Project Server peuvent avoir besoin d’être validés pour s’assurer qu’ils sont toujours correctement associés.</span><span class="sxs-lookup"><span data-stu-id="a6796-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
