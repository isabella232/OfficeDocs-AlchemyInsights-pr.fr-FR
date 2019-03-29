---
title: Restreindre SharePoint Online au mode classique
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30955985"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="ed949-102">Restreindre SharePoint Online au mode classique</span><span class="sxs-lookup"><span data-stu-id="ed949-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="ed949-103">Certaines organisations nécessitent toujours l'expérience en mode classique.</span><span class="sxs-lookup"><span data-stu-id="ed949-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="ed949-104">S'il n'est pas prévu de supprimer le mode classique à un niveau granulaire, à compter du 1er avril 2019, il n'est plus possible de limiter l'ensemble de l'organisation (client) au mode classique pour les listes et les bibliothèques.</span><span class="sxs-lookup"><span data-stu-id="ed949-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="ed949-105">Les options suivantes permettent aux administrateurs de gérer des listes et des bibliothèques individuelles en mode classique à l'aide de commutateurs d'exclusion granulaire que nous fournissons aux niveaux suivants:</span><span class="sxs-lookup"><span data-stu-id="ed949-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="ed949-106">collection de sites</span><span class="sxs-lookup"><span data-stu-id="ed949-106">site collection</span></span>
- <span data-ttu-id="ed949-107">site</span><span class="sxs-lookup"><span data-stu-id="ed949-107">site</span></span>
- <span data-ttu-id="ed949-108">liste</span><span class="sxs-lookup"><span data-stu-id="ed949-108">list</span></span>
- <span data-ttu-id="ed949-109">Bibliothèque</span><span class="sxs-lookup"><span data-stu-id="ed949-109">library</span></span>

<span data-ttu-id="ed949-110">En outre, les listes qui utilisent certaines fonctionnalités et personnalisations qui ne sont pas prises en charge par Modern seront toujours automatiquement basculées vers le mode classique.</span><span class="sxs-lookup"><span data-stu-id="ed949-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="ed949-111">Après le 1er avril, les listes et les bibliothèques qui sont en mode classique suite à l'exclusion du client seront automatiquement gérées au niveau du site et de la liste.</span><span class="sxs-lookup"><span data-stu-id="ed949-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="ed949-112">Si vous avez besoin du mode classique, reportez-vous à cette rubrique pour obtenir plus d'informations et des instructions PowerShell PnP ici qui décrivent les options et les outils que vous pouvez utiliser dès à présent pour préparer la suppression du niveau client opt-out le 1er avril.</span><span class="sxs-lookup"><span data-stu-id="ed949-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
