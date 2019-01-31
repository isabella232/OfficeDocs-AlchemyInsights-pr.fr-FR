---
title: Résoudre les problèmes à l’aide d’ouvrir avec l’Explorateur de solutions
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661749"
---
# <a name="fix-problems-with-open-with-explorer"></a>Résoudre les problèmes ouvrir dans l’Explorateur de solutions

Résoudre les problèmes courants liés à l’ouverture d’une bibliothèque de documents dans SharePoint ou à l’aide de la commande **Ouvrir avec l’Explorateur** de OneDrive : 
  
- Utiliser Internet Explorer 10 ou Internet Explorer 11. **Ouvrir avec l’Explorateur** n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres personnes. **Ouvrir avec l’Explorateur** est désactivé dans tous les navigateurs à l’exception d’Internet Explorer. 
    
- **Ouvrir avec l’Explorateur** n’est pas disponible dans l’expérience moderne pour les bibliothèques SharePoint. Utilisez **la vue dans l’Explorateur de fichiers** . Sélectionnez les **options d’affichage** \> **affichage dans l’Explorateur de fichiers**. Affichage dans l’Explorateur de fichiers n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres personnes. **Affichage dans l’Explorateur de fichiers** dans disponible uniquement dans Internet Explorer. 
    
- Assurez-vous que le service WebClient est en cours d’exécution. Dans la zone de recherche de Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services.msc, puis appuyez sur ENTRÉE. Faites défiler jusqu'à la service WebClient et assurez-vous que la colonne **état** affiche « En cours d’exécution. » Le cas contraire, double-cliquez sur le service, cliquez sur **Démarrer**, puis cliquez sur **OK**. (Vous devrez peut-être d’abord activer le service en sélectionnant l’option **manuel** ou **automatique** dans la zone **type de démarrage** ). 
    
> [!NOTE]
> Ouverture d’une bibliothèque dans l’Explorateur de fichiers est utile si vous souhaitez copier ou déplacer plusieurs fichiers et dossiers une fois, mais si vous souhaitez travailler régulièrement dans la bibliothèque, nous vous recommandons de synchroniser. Pour résoudre les problèmes d’ouverture dans l’Explorateur de fichiers, voir [Ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665). Pour obtenir des informations sur la configuration de synchronisation, consultez [les fichiers de synchronisation SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Consultez l’article [comment utiliser la commande « Ouvrir avec l’Explorateur » pour résoudre les problèmes dans SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) pour plus d’informations. 
  

