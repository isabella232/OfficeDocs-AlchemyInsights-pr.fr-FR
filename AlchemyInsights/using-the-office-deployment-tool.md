---
title: Utilisation de l’outil déploiement d’Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365523"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="d69b3-102">Utilisation de l’outil déploiement d’Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="d69b3-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d69b3-103">L’outil déploiement d’Office (ODT) vous permet de déployer des versions Office 365 d’Office.</span><span class="sxs-lookup"><span data-stu-id="d69b3-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="d69b3-104">L’outil déploiement d’Office (Setup. exe) est exécuté à partir de la ligne de commande et utilise un fichier XML de configuration pour déterminer les paramètres à appliquer lors du déploiement d’Office.</span><span class="sxs-lookup"><span data-stu-id="d69b3-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="d69b3-105">Téléchargez la dernière version de l’outil déploiement d’Office à partir du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="d69b3-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="d69b3-106">Utilisez l' [outil de personnalisation Office (OPO)](https://config.office.com) pour sélectionner vos préférences de déploiement et créer le fichier XML de configuration.</span><span class="sxs-lookup"><span data-stu-id="d69b3-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="d69b3-107">Exportez le fichier de configuration et placez-le localement dans le dossier où réside le programme Setup. exe.</span><span class="sxs-lookup"><span data-stu-id="d69b3-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="d69b3-108">**Remarque:** Les problèmes d’installation d’Office se produisent généralement en raison de fichiers de configuration mal configurés ou malformatted.</span><span class="sxs-lookup"><span data-stu-id="d69b3-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="d69b3-109">Pour éviter ces problèmes, nous vous recommandons d’utiliser l’outil de personnalisation Office pour créer le fichier de configuration.</span><span class="sxs-lookup"><span data-stu-id="d69b3-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="d69b3-110">Vous pouvez également importer des fichiers de configuration existants dans l’outil de personnalisation Office.</span><span class="sxs-lookup"><span data-stu-id="d69b3-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="d69b3-111">À partir d’une invite de commandes avec élévation de privilèges, basculez vers l’emplacement où Setup. exe réside et exécutez l’outil déploiement d’Office en mode de téléchargement, puis spécifiez le fichier de configuration que vous venez d’enregistrer.</span><span class="sxs-lookup"><span data-stu-id="d69b3-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="d69b3-112">Dans cet exemple, le fichier de configuration est nommé Configuration. xml:</span><span class="sxs-lookup"><span data-stu-id="d69b3-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="d69b3-113">Exécutez l’outil déploiement d’Office en mode de configuration et spécifiez le fichier de configuration.</span><span class="sxs-lookup"><span data-stu-id="d69b3-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="d69b3-114">**Remarque:** Vous devez exécuter cette étape à partir de l’ordinateur client sur lequel vous voulez installer Office et vous devez disposer des autorisations d’administrateur local sur cet ordinateur.</span><span class="sxs-lookup"><span data-stu-id="d69b3-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="d69b3-115">Pour en savoir plus sur l’utilisation de l’outil déploiement d’Office pour vos scénarios de déploiement d’Office 365 ProPlus, consultez [la rubrique vue d’ensemble de l’outil déploiement d’Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="d69b3-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="d69b3-116">Pour plus d’informations sur l’utilisation de l’outil de personnalisation Office, voir [vue d’ensemble de l’outil de personnalisation Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="d69b3-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
