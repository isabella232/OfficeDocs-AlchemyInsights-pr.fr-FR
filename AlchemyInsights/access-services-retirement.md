---
title: Déclassement Access services
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495749"
---
# <a name="access-services-retirement"></a><span data-ttu-id="f9520-102">Déclassement Access services</span><span class="sxs-lookup"><span data-stu-id="f9520-102">Access services retirement</span></span>

<span data-ttu-id="f9520-103">Comme nous l’avons annoncé à l’origine dans MC97576, en mars 2017, et continuait de communiquer au cours de l’année précédente, Access services est retiré de Office 365.</span><span class="sxs-lookup"><span data-stu-id="f9520-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="f9520-104">La phase suivante de ce processus est la suppression des bases de données Web Access qui utilisent des listes SharePoint comme stockage de données sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="f9520-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="f9520-105">**Comment cela m’affecte-t-il?**</span><span class="sxs-lookup"><span data-stu-id="f9520-105">**How does this affect me?**</span></span>

<span data-ttu-id="f9520-106">À partir du 2019 juin, nous allons arrêter la création de nouvelles bases de données Access dans SharePoint Online et arrêter le service et toutes les applications restantes d’avril 2020.</span><span class="sxs-lookup"><span data-stu-id="f9520-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="f9520-107">**Que dois-je faire pour préparer cette modification?**</span><span class="sxs-lookup"><span data-stu-id="f9520-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="f9520-108">Nous vous encourageons à créer un plan de transition pour les bases de données Web Access de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="f9520-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="f9520-109">Les administrateurs peuvent utiliser l’analyseur d' [applications SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pour obtenir un inventaire des applications Access que les sites utilisent.</span><span class="sxs-lookup"><span data-stu-id="f9520-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="f9520-110">Il existe plusieurs façons de migrer des données de bases de données Web Access:</span><span class="sxs-lookup"><span data-stu-id="f9520-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="f9520-111">Importation dans une base de données Access locale (. ACCDB) ou dans un fichier Excel.</span><span class="sxs-lookup"><span data-stu-id="f9520-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="f9520-112">Nous vous recommandons également d’explorer Microsoft PowerApps comme une autre plate-forme pour créer des solutions d’entreprise sans code pour le Web et les appareils mobiles.</span><span class="sxs-lookup"><span data-stu-id="f9520-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>