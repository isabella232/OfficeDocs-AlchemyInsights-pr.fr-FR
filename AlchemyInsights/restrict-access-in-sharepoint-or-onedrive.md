---
title: Restreindre l’accès dans SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551449"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a0e09-102">Restreindre l’accès dans SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="a0e09-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a0e09-103">Dans SharePoint et OneDrive, vous restreignez l’accès à des éléments tels que des fichiers, des dossiers et des listes en accordant uniquement l’accès à des groupes ou à des personnes auxquelles vous souhaitez accéder.</span><span class="sxs-lookup"><span data-stu-id="a0e09-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="a0e09-104">Par défaut, les autorisations dans SharePoint sont héritées d’un niveau supérieur dans la hiérarchie.</span><span class="sxs-lookup"><span data-stu-id="a0e09-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a0e09-105">Par conséquent, un fichier hérite ses autorisations du dossier, qui hérite ses autorisations de la bibliothèque, qui hérite ses autorisations du site.</span><span class="sxs-lookup"><span data-stu-id="a0e09-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="a0e09-106">Vous pouvez partager à un niveau supérieur (par exemple, en partageant un site entier), puis annuler l’héritage si vous ne souhaitez pas partager tous les éléments sur le site.</span><span class="sxs-lookup"><span data-stu-id="a0e09-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="a0e09-107">Toutefois, nous vous déconseillons de le faire car cela rend la maintenance des autorisations plus complexe et plus difficile à venir.</span><span class="sxs-lookup"><span data-stu-id="a0e09-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="a0e09-108">Voici ce que vous pouvez faire à la place:</span><span class="sxs-lookup"><span data-stu-id="a0e09-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="a0e09-109">Si, par exemple, vous souhaitez partager tout le contenu d’un dossier à l’exception d’un fichier qu’il contient, déplacez ce fichier vers un nouvel emplacement qui n’est pas partagé.</span><span class="sxs-lookup"><span data-stu-id="a0e09-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="a0e09-110">Si vous avez deux sous-dossiers dans un dossier et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement le groupe un à accéder au deuxième sous-dossier, partagez le dossier parent avec le groupe A et ajoutez le groupe B au premier sous-dossier.</span><span class="sxs-lookup"><span data-stu-id="a0e09-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="a0e09-111">Arrêter le partage d’un fichier ou d’un dossier</span><span class="sxs-lookup"><span data-stu-id="a0e09-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

