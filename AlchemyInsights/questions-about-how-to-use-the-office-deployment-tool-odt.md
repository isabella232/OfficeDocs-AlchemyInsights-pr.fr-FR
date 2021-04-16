---
title: Questions sur l'utilisation de l'outil Déploiement d'Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790330"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Questions sur l'utilisation de l'outil Déploiement d'Office (ODT)

Téléchargez l’outil Déploiement d’Office du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Après avoir téléchargé le fichier, exécutez le fichier exécutable auto-extractible qui contient le fichier exécutable de l’outil Déploiement d’Office (setup.exe) et un exemple de fichier de configuration (configuration.xml).
  
 **Pour exclure ou supprimer des produits Microsoft 365 Apps for enterprise des ordinateurs clients :**
  
Lors de l'installation de Microsoft 365 Apps pour entreprise, vous pouvez exclure des produits spécifiques. Pour ce faire, suivez la procédure d'installation d'Office avec l'outil Déploiement d'Office, mais incluez l'élément ExcludeApp dans votre fichier de configuration. Par exemple, ce fichier de configuration installe tous les produits Microsoft 365 Apps for enterprise, à l'exception de Publisher :
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Vue d’ensemble de l’outil Déploiement d’Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

