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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774889"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="37186-102">Questions sur l’utilisation de l’outil déploiement d’Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="37186-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="37186-103">Téléchargez l’outil Déploiement d’Office du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="37186-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="37186-104">Après avoir téléchargé le fichier, exécutez le fichier exécutable auto-extractible qui contient le fichier exécutable de l’outil Déploiement d’Office (setup.exe) et un exemple de fichier de configuration (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="37186-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="37186-105">**Pour exclure ou supprimer les applications Microsoft 365 pour les produits d’entreprise des ordinateurs clients :**</span><span class="sxs-lookup"><span data-stu-id="37186-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="37186-106">Lors de l’installation d’applications Microsoft 365 pour Enterprise, vous pouvez exclure des produits spécifiques.</span><span class="sxs-lookup"><span data-stu-id="37186-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="37186-107">Pour ce faire, suivez la procédure d'installation d'Office avec l'outil Déploiement d'Office, mais incluez l'élément ExcludeApp dans votre fichier de configuration.</span><span class="sxs-lookup"><span data-stu-id="37186-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="37186-108">Par exemple, ce fichier de configuration installe toutes les applications Microsoft 365 pour les produits d’entreprise, à l’exception de Publisher :</span><span class="sxs-lookup"><span data-stu-id="37186-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="37186-109">Vue d’ensemble de l’outil Déploiement d’Office</span><span class="sxs-lookup"><span data-stu-id="37186-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

