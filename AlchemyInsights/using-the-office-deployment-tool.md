---
title: Utilisation de l’outil Office Déploiement
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083768"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilisation de l’outil déploiement Office (ODT)

Vous utilisez l’outil déploiement Office (ODT) pour déployer Office 365 versions de Office. L’Office Deployment Tool (setup.exe) est exécuté à partir de la ligne de commande et utilise un fichier XML de configuration pour déterminer les paramètres à appliquer lors du déploiement de Office.
  
1. Téléchargez la dernière version de l’outil déploiement Office à partir du [Centre de téléchargement Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Utilisez [l Office PERSONNALISATION (PERSONNALISATION)](https://config.office.com) pour sélectionner vos préférences de déploiement et créer le fichier XML de configuration. Exportez le fichier de configuration et placez-le localement dans le même dossier que le setup.exe réside.

    **Remarque : Office’installation** se produisent généralement en raison de fichiers de configuration mal configurés ou mal configurés. Pour éviter de tels problèmes, nous vous recommandons d’utiliser Office outil de personnalisation pour créer le fichier de configuration. Vous pouvez également importer des fichiers de configuration existants dans l Office de personnalisation.

3. À partir d’une invite de commandes avec élévation de setup.exe, exécutez l’outil déploiement Office en mode de téléchargement et spécifiez le fichier de configuration que vous avez enregistré. Dans cet exemple, le fichier de configuration est nommé Configuration.xml :

```setup.exe /download Configuration.xml```

4.Exécutez l’outil Office déploiement en mode de configuration et spécifiez le fichier de configuration.

```setup.exe /configure Configuration.xml```

**Remarque :** Vous devez exécuter cette étape à partir de l’ordinateur client sur lequel vous souhaitez installer Office et vous devez avoir des autorisations d’administrateur local sur cet ordinateur.

Pour en savoir plus sur l Office de déploiement pour vos scénarios de déploiement Applications Microsoft 365 pour les grandes entreprises, voir Vue d’ensemble de l Office [de déploiement.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Pour plus d’informations sur l’utilisation de l Office de personnalisation, voir Vue d’ensemble de [l’outil Office Personnalisation.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
