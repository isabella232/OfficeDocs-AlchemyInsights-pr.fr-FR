---
title: Déclassement Access services
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973916"
---
# <a name="access-services-retirement"></a><span data-ttu-id="926fb-102">Déclassement Access services</span><span class="sxs-lookup"><span data-stu-id="926fb-102">Access services retirement</span></span>

<span data-ttu-id="926fb-103">Comme nous l’avons annoncé à l’origine dans MC97576, en mars 2017, et continuait de communiquer au cours de l’année précédente, Access services est retiré de Office 365.</span><span class="sxs-lookup"><span data-stu-id="926fb-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="926fb-104">La phase suivante de ce processus est la suppression des bases de données Web Access qui utilisent des listes SharePoint comme stockage de données sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="926fb-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="926fb-105">Comment cela m’affecte-t-il?</span><span class="sxs-lookup"><span data-stu-id="926fb-105">How does this affect me?</span></span>

<span data-ttu-id="926fb-106">À partir du 2019 juin, nous allons arrêter la création de nouvelles bases de données Access dans SharePoint Online et arrêter le service et toutes les applications restantes d’avril 2020.</span><span class="sxs-lookup"><span data-stu-id="926fb-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="926fb-107">Que dois-je faire pour préparer cette modification?</span><span class="sxs-lookup"><span data-stu-id="926fb-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="926fb-108">Nous vous encourageons à créer un plan de transition pour les bases de données Web Access de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="926fb-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="926fb-109">Les administrateurs peuvent utiliser l’analyseur d' [applications SharePoint Access](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) pour obtenir un inventaire des applications Access que les sites utilisent.</span><span class="sxs-lookup"><span data-stu-id="926fb-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="926fb-110">Il existe plusieurs façons de migrer des données de bases de données Web Access:</span><span class="sxs-lookup"><span data-stu-id="926fb-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="926fb-111">Importation dans une base de données Access locale (. ACCDB) ou dans un fichier Excel.</span><span class="sxs-lookup"><span data-stu-id="926fb-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="926fb-112">Nous vous recommandons également d’explorer Microsoft PowerApps comme une autre plate-forme pour créer des solutions d’entreprise sans code pour le Web et les appareils mobiles.</span><span class="sxs-lookup"><span data-stu-id="926fb-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>