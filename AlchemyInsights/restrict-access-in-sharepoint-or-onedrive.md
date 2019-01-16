---
title: Restreindre l’accès dans SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288459"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="5fb0b-102">Restreindre l’accès dans SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="5fb0b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="5fb0b-p101">Dans SharePoint et OneDrive, vous restreindre l’accès aux éléments de listes, dossiers et fichiers à accorder l’accès uniquement à des groupes ou des personnes que vous souhaitez accéder. Par défaut, les autorisations dans SharePoint héritées de plus haut dans la hiérarchie. Si un fichier hérite ses autorisations du dossier, qui hérite ses autorisations de la bibliothèque qui hérite ses autorisations du site.</span><span class="sxs-lookup"><span data-stu-id="5fb0b-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="5fb0b-p102">Vous pouvez partager à un niveau supérieur (telle que par la totalité d’un site de partage), puis rompre l’héritage des autorisations si vous ne souhaitez pas partager tous les éléments sur le site. Toutefois, n’est pas recommandé cela car elle permet la gestion des autorisations plus complexe et difficile à l’avenir. Voici comment procéder à la place :</span><span class="sxs-lookup"><span data-stu-id="5fb0b-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="5fb0b-109">Si, par exemple, vous souhaitez partager tout le contenu d’un dossier à l’exception d’un seul fichier, déplacez ce fichier vers un nouvel emplacement qui n’est pas partagé.</span><span class="sxs-lookup"><span data-stu-id="5fb0b-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="5fb0b-110">Si vous avez deux sous-dossiers dans un dossier, et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement l’accès vers le sous-dossier deuxième groupe A, partagez le dossier parent avec groupe A et ajouter le groupe B vers le sous-dossier premier.</span><span class="sxs-lookup"><span data-stu-id="5fb0b-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="5fb0b-111">Arrêter de partager un fichier ou un dossier</span><span class="sxs-lookup"><span data-stu-id="5fb0b-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

