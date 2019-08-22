---
title: Le partage avec des utilisateurs externes ne fonctionne pas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502229"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Résoudre les problèmes de partage de contenu SharePoint avec des utilisateurs externes

Assurez-vous que le partage externe est activé pour votre organisation:
  
1. Accédez à la [page &amp; compléments de services dans le centre d’administration 365 de Microsoft](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), puis cliquez sur **sites**.
    
2. Assurez-vous que le paramètre est activé. Si «uniquement les utilisateurs externes existants» est sélectionné, assurez-vous que l’utilisateur externe est affiché dans le centre d’administration 365 de Microsoft.
    
Assurez-vous que le partage externe est activé pour le site. Pour une collection de sites classique:
  
1. Dans le nouveau centre d’administration SharePoint, dans le volet de gauche, cliquez sur **sites**.
    
2. Sélectionnez le ou les sites et, dans le ruban, cliquez sur **partage**.
    
Pour un site d’équipe appartenant à un groupe Office 365 ou à un site de communication:
  
- Ces nouveaux types de sites ont le même paramètre de partage que votre paramètre à l’échelle de votre organisation, sauf si le paramètre à l’échelle de l’organisation autorise le partage de fichiers à l’aide de liens ne nécessitant pas de connexion. Dans ce cas, les sites autorisent le partage avec des utilisateurs externes nouveaux et existants qui se connectent. Pour modifier le paramètre de sites spécifiques, utilisez le nouveau centre d’administration SharePoint ou PowerShell. [En savoir plus](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Le paramètre de partage externe de n’importe quel site peut être plus restrictif que le paramètre à l’échelle de votre organisation, mais pas plus permissif que le paramètre à l’échelle de l’organisation. 
  

