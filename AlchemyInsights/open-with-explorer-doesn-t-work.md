---
title: Ouvrir avec l’Explorateur ne fonctionne pas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321859"
---
# <a name="open-with-explorer-isnt-working"></a>Ouvrir avec l’Explorateur ne fonctionne pas

Si **Ouvrir avec l’Explorateur** ou Afficher dans l’Explorateur de fichiers  ne fonctionne pas, assurez-vous que le service WebClient est en cours d’exécution en suivant les étapes ci-dessous.  Par exemple, l’ouverture d’une bibliothèque SharePoint bibliothèque OneDrive peut prendre du temps lorsque le service n’est pas en cours d’exécution. 
  
1. Dans la Windows de recherche, tapez Exécuter, sélectionnez Exécuter l’application de bureau Exécuter, tapez services.msc, puis sélectionnez **Entrée**.
    
2. Faites défiler vers le bas jusqu’au service WebClient et vérifiez la **colonne État.** Si l’état du service WebClient n’est pas en cours d’exécution, double-cliquez sur le service, cliquez sur **Démarrer,** puis sur **OK**. Activez le service, si nécessaire, en sélectionnant Manuel ou **Automatique** dans la zone **De démarrage.**  
    
**Remarque**: pour résoudre les problèmes d’ouverture dans l’Explorateur de fichiers, voir [Ouvrir dans l’Explorateur.](https://go.microsoft.com/fwlink/?linkid=871665) Explorez la synchronisation comme meilleure alternative : [synchronisez SharePoint fichiers avec le nouveau client Synchronisation OneDrive client.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

