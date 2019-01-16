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
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restreindre l’accès dans SharePoint ou OneDrive

Dans SharePoint et OneDrive, vous restreindre l’accès aux éléments de listes, dossiers et fichiers à accorder l’accès uniquement à des groupes ou des personnes que vous souhaitez accéder. Par défaut, les autorisations dans SharePoint héritées de plus haut dans la hiérarchie. Si un fichier hérite ses autorisations du dossier, qui hérite ses autorisations de la bibliothèque qui hérite ses autorisations du site.
  
Vous pouvez partager à un niveau supérieur (telle que par la totalité d’un site de partage), puis rompre l’héritage des autorisations si vous ne souhaitez pas partager tous les éléments sur le site. Toutefois, n’est pas recommandé cela car elle permet la gestion des autorisations plus complexe et difficile à l’avenir. Voici comment procéder à la place :
  
- Si, par exemple, vous souhaitez partager tout le contenu d’un dossier à l’exception d’un seul fichier, déplacez ce fichier vers un nouvel emplacement qui n’est pas partagé.
    
- Si vous avez deux sous-dossiers dans un dossier, et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement l’accès vers le sous-dossier deuxième groupe A, partagez le dossier parent avec groupe A et ajouter le groupe B vers le sous-dossier premier.
    
[Arrêter de partager un fichier ou un dossier](https://go.microsoft.com/fwlink/?linkid=2008861)
  

