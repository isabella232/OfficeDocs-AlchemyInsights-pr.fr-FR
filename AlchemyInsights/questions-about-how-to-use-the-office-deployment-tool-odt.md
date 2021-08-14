---
title: Questions sur l’utilisation de l’outil déploiement Office (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959681"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Questions sur l’utilisation de l’outil déploiement Office (ODT)

Téléchargez l’outil Déploiement d’Office du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Après avoir téléchargé le fichier, exécutez le fichier exécutable auto-extractible qui contient le fichier exécutable de l’outil Déploiement d’Office (setup.exe) et un exemple de fichier de configuration (configuration.xml).
  
 **Pour exclure ou supprimer des Applications Microsoft 365 pour les grandes entreprises d’ordinateurs clients :**
  
Lors de l’installation Applications Microsoft 365 pour les grandes entreprises, vous pouvez exclure des produits spécifiques. Pour ce faire, suivez la procédure d'installation d'Office avec l'outil Déploiement d'Office, mais incluez l'élément ExcludeApp dans votre fichier de configuration. Par exemple, ce fichier de configuration installe tous les produits Applications Microsoft 365 pour les grandes entreprises à l’exception Publisher :
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Vue d’ensemble de l’outil Déploiement d’Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

