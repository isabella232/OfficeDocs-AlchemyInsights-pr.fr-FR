---
title: Restreindre l'accès dans SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383869"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restreindre l'accès dans SharePoint ou OneDrive

Dans SharePoint et OneDrive, vous restreignez l'accès à des éléments tels que des fichiers, des dossiers et des listes en accordant uniquement l'accès à des groupes ou à des personnes auxquelles vous souhaitez accéder. Par défaut, les autorisations dans SharePoint sont héritées d'un niveau supérieur dans la hiérarchie. Par conséquent, un fichier hérite ses autorisations du dossier, qui hérite ses autorisations de la bibliothèque, qui hérite ses autorisations du site.
  
Vous pouvez partager à un niveau supérieur (par exemple, en partageant un site entier), puis annuler l'héritage si vous ne souhaitez pas partager tous les éléments sur le site. Toutefois, nous vous déconseillons de le faire car cela rend la maintenance des autorisations plus complexe et plus difficile à venir. Voici ce que vous pouvez faire à la place:
  
- Si, par exemple, vous souhaitez partager tout le contenu d'un dossier à l'exception d'un fichier qu'il contient, déplacez ce fichier vers un nouvel emplacement qui n'est pas partagé.
    
- Si vous avez deux sous-dossiers dans un dossier et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement le groupe un à accéder au deuxième sous-dossier, partagez le dossier parent avec le groupe A et ajoutez le groupe B au premier sous-dossier.
    
[Arrêter le partage d'un fichier ou d'un dossier](https://go.microsoft.com/fwlink/?linkid=2008861)
  

