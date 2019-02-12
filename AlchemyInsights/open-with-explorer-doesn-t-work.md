---
title: Ouvrir dans l’Explorateur de solutions ne fonctionne pas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906802"
---
# <a name="open-with-explorer-isnt-working"></a>Ouvrir dans l’Explorateur de solutions ne fonctionne pas

Si **Ouvrir avec l’Explorateur** ou **affichage dans l’Explorateur de fichiers** ne fonctionne pas, assurez-vous que le service WebClient est en cours **d’exécution** en suivant les étapes ci-dessous. Par exemple, il peut prendre beaucoup de temps pour ouvrir une bibliothèque SharePoint ou OneDrive lorsque le service n’est pas en cours d’exécution. 
  
1. Dans la zone de recherche de Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services.msc et puis sélectionnez **entrée**.
    
2. Faites défiler jusqu'à la service WebClient et vérifiez la colonne **état** . Si l’état du service WebClient n’est pas **en cours d’exécution**, double-cliquez sur le service, cliquez sur **Démarrer**, puis cliquez sur **OK**. Activez le service, le cas échéant, en sélectionnant l’option **manuel** ou **automatique** dans la zone **type de démarrage** . 
    
> [!NOTE]
> Pour résoudre les problèmes d’ouverture dans l’Explorateur de fichiers, voir [Ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665). Explorez la synchronisation comme une meilleure solution : [fichiers de synchronisation SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

