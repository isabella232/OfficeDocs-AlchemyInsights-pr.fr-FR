---
title: Ouvrir avec l'Explorateur ne fonctionne pas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419869"
---
# <a name="open-with-explorer-isnt-working"></a>Ouvrir avec l'Explorateur ne fonctionne pas

Si **Ouvrir avec l'Explorateur** ou **afficher dans l'Explorateur de fichiers** ne fonctionne pas, vérifiez que le service WebClient est configuré pour **s'exécuter** en suivant les étapes ci-dessous. Par exemple, l'ouverture d'une bibliothèque SharePoint ou OneDrive peut prendre beaucoup de temps lorsque le service n'est pas en cours d'exécution. 
  
1. Dans la zone de recherche Windows, tapez exécuter, sélectionnez l'application de bureau exécuter, tapez services. msc, puis appuyez sur **entrée**.
    
2. Faites déFiler vers le bas jusqu'au service webClient et vérifiez la colonne **État** . Si l'état du service webClient n'est pas **en cours d'exécution**, double-cliquez sur le service, cliquez sur **Démarrer**, puis sur **OK**. Activez le service, le cas échéant, en sélectionnant **Manuel** ou **automatique** dans la zone **type de démarrage** . 
    
> [!NOTE]
> Pour résoudre les problèmes qui s'ouvrent dans l'Explorateur de fichiers, consultez la rubrique [ouvrir dans l'Explorateur](https://go.microsoft.com/fwlink/?linkid=871665). Explorez la synchronisation en tant qu'alternative plus efficace: [synchroniser les fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

