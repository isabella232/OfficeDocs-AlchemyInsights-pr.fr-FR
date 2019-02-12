---
title: Questions sur l’utilisation de l’outil de déploiement d’Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925342"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="ae9d5-102">Questions sur l’utilisation de l’outil de déploiement d’Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="ae9d5-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ae9d5-103">Téléchargez l’outil Déploiement d’Office du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ae9d5-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="ae9d5-104">Après avoir téléchargé le fichier, exécutez le fichier exécutable auto-extractible qui contient le fichier exécutable de l’outil Déploiement d’Office (setup.exe) et un exemple de fichier de configuration (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="ae9d5-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="ae9d5-105">**Pour exclure ou supprimer des produits Office 365 ProPlus à partir des ordinateurs clients :**</span><span class="sxs-lookup"><span data-stu-id="ae9d5-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="ae9d5-p101">Pendant l’installation d’Office 365 ProPlus, vous pouvez exclure des produits spécifiques. Pour ce faire, suivez la procédure d’installation d’Office avec ODT, mais incluez l’élément ExcludeApp dans votre fichier de configuration. Par exemple, ce fichier de configuration installe tous les produits Office 365 ProPlus à l’exception du serveur de publication :</span><span class="sxs-lookup"><span data-stu-id="ae9d5-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="ae9d5-109">Vue d’ensemble de l’outil Déploiement d’Office</span><span class="sxs-lookup"><span data-stu-id="ae9d5-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

