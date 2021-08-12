---
title: Le partage avec des utilisateurs externes ne fonctionne pas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910364"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Résoudre les problèmes de partage SharePoint contenu avec des utilisateurs externes

Assurez-vous que le partage externe est allumé pour votre organisation :
  
1. Go to the [Services &amp; add-ins page in the Centre d’administration Microsoft 365,](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)and click **Sites**.
    
2. Assurez-vous que le paramètre est désactivé. Si « Seuls les utilisateurs externes existants » sont sélectionnés, assurez-vous que l’utilisateur externe est répertorié dans le Centre d’administration Microsoft 365.
    
Assurez-vous que le partage externe est allumé pour le site. Pour une collection de sites classique :
  
1. Dans le nouveau centre SharePoint’administration, dans le volet gauche, cliquez sur **sites.**
    
2. Sélectionnez le ou les sites, puis dans le ruban, cliquez sur **Partage.**
    
Pour un site d’équipe qui appartient à un groupe Microsoft 365 ou un site de communication :
  
- Ces nouveaux types de sites ont le même paramètre de partage que le paramètre à l’échelle de votre organisation, sauf si le paramètre à l’échelle de l’organisation autorise le partage de fichiers à l’aide de liens qui ne nécessitent pas de se connecter. Dans ce cas, les sites autorisent le partage avec les utilisateurs externes nouveaux et existants qui se connectent. Pour modifier le paramètre pour des sites spécifiques, utilisez le nouveau centre d’administration SharePoint ou PowerShell. [En savoir plus](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Le paramètre de partage externe pour n’importe quel site peut être plus restrictif que le paramètre à l’échelle de votre organisation, mais pas plus permissif que le paramètre à l’échelle de l’organisation. 
  

