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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011334"
---
# <a name="open-with-explorer-isnt-working"></a>Ouvrir avec l’Explorateur ne fonctionne pas

Si **Ouvrir avec l’Explorateur** ou Afficher dans l’Explorateur de fichiers  ne fonctionne pas, assurez-vous que le service WebClient est bien en cours d’exécution en suivant les étapes ci-dessous.  Par exemple, l’ouverture d’une bibliothèque SharePoint bibliothèque OneDrive peut prendre du temps lorsque le service n’est pas en cours d’exécution. 
  
1. Dans la Windows recherche, tapez Exécuter, sélectionnez Exécuter l’application de bureau Exécuter, tapez services.msc, puis sélectionnez **Entrée**.
    
2. Faites défiler vers le bas jusqu’au service WebClient et vérifiez la **colonne État.** Si l’état du service WebClient n’est pas en cours d’exécution, double-cliquez sur le service, cliquez sur **Démarrer,** puis sur **OK**. Activez le service, si nécessaire, en sélectionnant Manuel ou **Automatique** dans la zone **De démarrage.**  
    
> [!NOTE]
> Pour résoudre les problèmes d’ouverture dans l’Explorateur de fichiers, voir [Ouvrir dans l’Explorateur.](https://go.microsoft.com/fwlink/?linkid=871665) Explorez la synchronisation comme meilleure alternative : [synchronisez SharePoint fichiers avec le nouveau client Synchronisation OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

