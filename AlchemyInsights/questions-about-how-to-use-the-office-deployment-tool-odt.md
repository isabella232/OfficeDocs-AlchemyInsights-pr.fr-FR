---
title: Questions sur l’utilisation de l’outil déploiement d’Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086154"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Questions sur l’utilisation de l’outil déploiement d’Office (ODT)

Téléchargez l’outil Déploiement d’Office du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Après avoir téléchargé le fichier, exécutez le fichier exécutable auto-extractible qui contient le fichier exécutable de l’outil déploiement d’Office (setupodt.exe) et un exemple de fichier de configuration (configuration.xml).
  
 **Pour exclure ou supprimer les applications Microsoft 365 pour les produits d’entreprise des ordinateurs clients :**
  
Lors de l’installation d’applications Microsoft 365 pour Enterprise, vous pouvez exclure des produits spécifiques. Pour ce faire, suivez la procédure d'installation d'Office avec l'outil Déploiement d'Office, mais incluez l'élément ExcludeApp dans votre fichier de configuration. Par exemple, ce fichier de configuration installe toutes les applications Microsoft 365 pour les produits d’entreprise, à l’exception de Publisher :
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Vue d’ensemble de l’outil Déploiement d’Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

