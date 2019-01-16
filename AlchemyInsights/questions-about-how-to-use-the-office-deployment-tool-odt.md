---
title: Questions sur l’utilisation de l’outil de déploiement d’Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287667"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Questions sur l’utilisation de l’outil de déploiement d’Office (ODT)

Téléchargez l’outil Déploiement d’Office du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Après avoir téléchargé le fichier, exécutez le fichier exécutable auto-extractible qui contient le fichier exécutable de l’outil Déploiement d’Office (setup.exe) et un exemple de fichier de configuration (configuration.xml).
  
 **Pour exclure ou supprimer des produits Office 365 ProPlus à partir des ordinateurs clients :**
  
Pendant l’installation d’Office 365 ProPlus, vous pouvez exclure des produits spécifiques. Pour ce faire, suivez la procédure d’installation d’Office avec ODT, mais incluez l’élément ExcludeApp dans votre fichier de configuration. Par exemple, ce fichier de configuration installe tous les produits Office 365 ProPlus à l’exception du serveur de publication :
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Vue d’ensemble de l’outil Déploiement d’Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

