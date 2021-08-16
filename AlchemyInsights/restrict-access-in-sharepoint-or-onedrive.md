---
title: Restreindre l’accès dans SharePoint ou OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075038"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restreindre l’accès dans SharePoint ou OneDrive

Dans SharePoint et OneDrive, vous restreignez l’accès à des éléments tels que des fichiers, des dossiers et des listes en accordant l’accès uniquement aux groupes ou aux personnes à qui vous souhaitez accéder. Par défaut, les autorisations SharePoint sont héritées de niveau supérieur dans la hiérarchie. Un fichier hérite donc de ses autorisations du dossier, qui hérite de ses autorisations de la bibliothèque, qui hérite de ses autorisations du site.
  
Vous pouvez partager à un niveau supérieur (par exemple, en partageant un site entier), puis rompre l’héritage si vous ne souhaitez pas partager tous les éléments sur le site. Toutefois, cela n’est pas recommandé, car cela rend la maintenance des autorisations plus complexe et confuse à l’avenir. Voici ce que vous pouvez faire à la place :
  
- Si, par exemple, vous souhaitez partager tout le contenu d’un dossier à l’exception d’un fichier dans celui-ci, déplacez ce fichier vers un nouvel emplacement qui n’est pas partagé.
    
- Si vous avez deux sous-dossiers dans un dossier et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement le groupe A à accéder au deuxième sous-dossier, partagez le dossier parent avec le groupe A et ajoutez le groupe B au premier sous-dossier.
    
[Arrêter le partage d’un fichier ou d’un dossier ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

