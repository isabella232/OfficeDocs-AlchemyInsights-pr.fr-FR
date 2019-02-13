---
title: Partage avec des utilisateurs externes ne fonctionne pas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900866"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Résoudre les problèmes de partage de contenu SharePoint avec des utilisateurs externes

Assurez-vous que le partage externe est activé pour votre organisation :
  
1. Accédez à la [Services &amp; page des compléments dans le centre d’administration Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), cliquez sur **Sites**.
    
2. Assurez-vous que le paramètre est activé sur « On ». Si « Utilisateurs externes existants uniquement » sont sélectionnées, assurez-vous que l’utilisateur externe est répertorié dans le centre d’administration d’Office 365.
    
Assurez-vous qu’externe partage activé pour le site. Pour une collection de sites classique :
  
1. Dans le centre d’administration SharePoint classique, dans le volet gauche, cliquez sur **des collections de sites**.
    
2. Sélectionnez l’ou les sites, dans le ruban, cliquez sur **partage**.
    
Pour un site d’équipe qui appartient à un groupe d’Office 365, ou un site de communication :
  
- Ces nouveaux types de sites ont le même paramètre partage en tant que paramètre de l’échelle de l’organisation, à moins que le paramètre d’échelle de l’organisation permet le partage de fichiers à l’aide de liens qui ne nécessitent pas de connexion. Dans ce cas, les sites autoriser le partage avec des utilisateurs externes qui se connectent à. Pour modifier le paramètre pour des sites spécifiques, utilisez le nouveau centre d’administration SharePoint (preview) ou PowerShell. [En savoir plus](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Le paramètre partage externe pour un site peut être plus restrictif que votre paramètre de l’organisation, mais pas plus permissif que le paramètre de l’organisation. 
  

