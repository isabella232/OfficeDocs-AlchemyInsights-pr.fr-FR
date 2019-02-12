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
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905146"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restreindre l’accès dans SharePoint ou OneDrive

Dans SharePoint et OneDrive, vous restreindre l’accès aux éléments de listes, dossiers et fichiers à accorder l’accès uniquement à des groupes ou des personnes que vous souhaitez accéder. Par défaut, les autorisations dans SharePoint héritées de plus haut dans la hiérarchie. Si un fichier hérite ses autorisations du dossier, qui hérite ses autorisations de la bibliothèque qui hérite ses autorisations du site.
  
Vous pouvez partager à un niveau supérieur (telle que par la totalité d’un site de partage), puis rompre l’héritage des autorisations si vous ne souhaitez pas partager tous les éléments sur le site. Toutefois, n’est pas recommandé cela car elle permet la gestion des autorisations plus complexe et difficile à l’avenir. Voici comment procéder à la place :
  
- Si, par exemple, vous souhaitez partager tout le contenu d’un dossier à l’exception d’un seul fichier, déplacez ce fichier vers un nouvel emplacement qui n’est pas partagé.
    
- Si vous avez deux sous-dossiers dans un dossier, et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement l’accès vers le sous-dossier deuxième groupe A, partagez le dossier parent avec groupe A et ajouter le groupe B vers le sous-dossier premier.
    
[Arrêter de partager un fichier ou un dossier](https://go.microsoft.com/fwlink/?linkid=2008861)
  

