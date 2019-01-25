---
title: À l’aide de l’outil de déploiement d’Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468617"
---
# <a name="using-the-office-deployment-tool-odt"></a>À l’aide de l’outil de déploiement d’Office (ODT)

Vous utilisez l’outil de déploiement d’Office (ODT) pour déployer Office 365 les versions d’Office. L’outil de déploiement d’Office (setup.exe) est exécutée à partir de la ligne de commande et utilise un fichier XML de configuration pour déterminer les paramètres à appliquer lors du déploiement d’Office.
  
1. Télécharger la dernière version de l’outil de déploiement d’Office à partir du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Utilisez l' [Outil de personnalisation Office (OPO)](https://config.office.com) pour sélectionner vos préférences de déploiement et de créer le fichier XML de configuration. Exporter le fichier de configuration et le placer localement sur le même dossier où réside le setup.exe. 
    
    **Remarque :** Installation d’Office couramment des problèmes dus à mal configuré ou mal formatées les fichiers de configuration. Pour éviter ces problèmes, nous vous recommandons d’utiliser l’outil de personnalisation Office pour créer le fichier de configuration. Vous pouvez également importer des fichiers de configuration existants dans l’outil de personnalisation Office. 
    
3. À partir d’une invite de commandes avec élévation de privilèges, basculez vers l’emplacement où réside setup.exe et exécuter l’outil de déploiement d’Office en mode de téléchargement et spécifier le fichier de configuration que vous venez d’enregistrer. Dans cet exemple, le fichier de configuration est nommé Configuration.xml :
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Exécuter l’outil de déploiement d’Office en mode configure et spécifier le fichier de configuration.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Remarque :** Vous devez exécuter cette étape à partir de l’ordinateur client sur lequel vous voulez installer Office, et vous devez disposer des autorisations d’administrateur local sur cet ordinateur. 
    
Pour plus d’informations sur l’utilisation d’outil de déploiement d’Office pour vos scénarios de déploiement Office 365 ProPlus, voir [vue d’ensemble de l’outil de déploiement d’Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Pour plus d’informations sur la façon d’utiliser l’outil de personnalisation Office, voir [vue d’ensemble de l’outil de personnalisation Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

