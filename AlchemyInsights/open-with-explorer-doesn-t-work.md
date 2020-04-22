---
title: Ouvrir avec l’Explorateur ne fonctionne pas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713032"
---
# <a name="open-with-explorer-isnt-working"></a>Ouvrir avec l’Explorateur ne fonctionne pas

Si **Ouvrir avec l’Explorateur** ou **afficher dans l’Explorateur de fichiers** ne fonctionne pas, vérifiez que le service WebClient est configuré pour **s’exécuter** en suivant les étapes ci-dessous. Par exemple, l’ouverture d’une bibliothèque SharePoint ou OneDrive peut prendre beaucoup de temps lorsque le service n’est pas en cours d’exécution. 
  
1. Dans la zone de recherche Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services. msc, puis appuyez sur **entrée**.
    
2. Faites défiler vers le bas jusqu’au service WebClient et vérifiez la colonne **État** . Si l’état du service WebClient n’est pas **en cours d’exécution**, double-cliquez sur le service, cliquez sur **Démarrer**, puis sur **OK**. Activez le service, le cas échéant, en sélectionnant **Manuel** ou **automatique** dans la zone **type de démarrage** . 
    
> [!NOTE]
> Pour résoudre les problèmes qui s’ouvrent dans l’Explorateur de fichiers, consultez la rubrique [ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665). Explorez la synchronisation en tant qu’alternative plus efficace : [synchroniser les fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

