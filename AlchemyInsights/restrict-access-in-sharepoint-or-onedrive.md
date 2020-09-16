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
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720680"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restreindre l’accès dans SharePoint ou OneDrive

Dans SharePoint et OneDrive, vous restreignez l’accès à des éléments tels que des fichiers, des dossiers et des listes en accordant uniquement l’accès à des groupes ou à des personnes auxquelles vous souhaitez accéder. Par défaut, les autorisations dans SharePoint sont héritées d’un niveau supérieur dans la hiérarchie. Par conséquent, un fichier hérite ses autorisations du dossier, qui hérite ses autorisations de la bibliothèque, qui hérite ses autorisations du site.
  
Vous pouvez partager à un niveau supérieur (par exemple, en partageant un site entier), puis annuler l’héritage si vous ne souhaitez pas partager tous les éléments sur le site. Toutefois, nous vous déconseillons de le faire car cela rend la maintenance des autorisations plus complexe et plus difficile à venir. Voici ce que vous pouvez faire à la place :
  
- Si, par exemple, vous souhaitez partager tout le contenu d’un dossier à l’exception d’un fichier qu’il contient, déplacez ce fichier vers un nouvel emplacement qui n’est pas partagé.
    
- Si vous avez deux sous-dossiers dans un dossier et que vous souhaitez partager un sous-dossier avec les groupes A et B et autoriser uniquement le groupe un à accéder au deuxième sous-dossier, partagez le dossier parent avec le groupe A et ajoutez le groupe B au premier sous-dossier.
    
[Arrêter le partage d’un fichier ou d’un dossier ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

