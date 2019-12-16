---
title: Restreindre SharePoint Online au mode classique
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048758"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="7eeeb-102">Restreindre SharePoint Online au mode classique</span><span class="sxs-lookup"><span data-stu-id="7eeeb-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="7eeeb-103">Certaines organisations nécessitent toujours l’expérience en mode classique.</span><span class="sxs-lookup"><span data-stu-id="7eeeb-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="7eeeb-104">Même s’il n’est pas prévu de supprimer le mode classique à un niveau granulaire, il n’est plus possible de limiter l’ensemble de l’organisation (client) au mode classique pour les listes et les bibliothèques.</span><span class="sxs-lookup"><span data-stu-id="7eeeb-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="7eeeb-105">Les options suivantes permettent aux administrateurs de gérer des listes et des bibliothèques individuelles en mode classique à l’aide de commutateurs d’exclusion granulaire que nous fournissons aux niveaux suivants :</span><span class="sxs-lookup"><span data-stu-id="7eeeb-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="7eeeb-106">collection de sites</span><span class="sxs-lookup"><span data-stu-id="7eeeb-106">site collection</span></span>
- <span data-ttu-id="7eeeb-107">site</span><span class="sxs-lookup"><span data-stu-id="7eeeb-107">site</span></span>
- <span data-ttu-id="7eeeb-108">liste</span><span class="sxs-lookup"><span data-stu-id="7eeeb-108">list</span></span>
- <span data-ttu-id="7eeeb-109">Bibliothèque</span><span class="sxs-lookup"><span data-stu-id="7eeeb-109">library</span></span>

<span data-ttu-id="7eeeb-110">En outre, les listes qui utilisent certaines fonctionnalités et personnalisations qui ne sont pas prises en charge par Modern seront toujours automatiquement basculées vers le mode classique.</span><span class="sxs-lookup"><span data-stu-id="7eeeb-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="7eeeb-111">À partir du 1er avril 2019, le processus de désactivation de la liste et des bibliothèques modernes démarrera et continuera le 31 mai 2019.</span><span class="sxs-lookup"><span data-stu-id="7eeeb-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="7eeeb-112">Les listes et les bibliothèques en mode classique, à la suite de l’exclusion client, sont automatiquement déplacées vers la version moderne.</span><span class="sxs-lookup"><span data-stu-id="7eeeb-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="7eeeb-113">Si vous avez besoin du mode classique, reportez-vous à cette rubrique pour obtenir plus [d’informations et](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) des instructions PowerShell PNP [ici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) qui décrit les options et les outils que vous pouvez utiliser aujourd’hui pour utiliser l’expérience en mode classique.</span><span class="sxs-lookup"><span data-stu-id="7eeeb-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
