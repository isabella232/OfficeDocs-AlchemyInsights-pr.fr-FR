---
title: Résoudre les problèmes à l’aide de l’outil Ouvrir avec l’Explorateur
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048154"
---
# <a name="fix-problems-with-open-with-explorer"></a>Résoudre les problèmes liés à l’ouverture avec l’Explorateur

Résoudre les problèmes courants liés à l’ouverture d’une bibliothèque de documents SharePoint ou OneDrive l’aide de la commande Ouvrir **avec l’Explorateur** : 
  
- Utilisez Internet Explorer 10 ou Internet Explorer 11. **Ouvrir avec l’Explorateur** n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres. **L’ouverture avec l’Explorateur** est désactivée dans tous les navigateurs à l’exception d’Internet Explorer. 
    
- **Ouvrir avec l’Explorateur** n’est pas disponible dans l’expérience moderne pour SharePoint bibliothèques. Utilisez **plutôt l’affichage dans l’Explorateur** de fichiers. Sélectionnez **Afficher les options** \> **d’affichage dans l’Explorateur de fichiers.** L’affichage dans l’Explorateur de fichiers n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres. **Affichage dans l’Explorateur de** fichiers disponible uniquement dans Internet Explorer. 
    
- Assurez-vous que le service WebClient est en cours d’exécution. Dans la Windows recherche, tapez Exécuter, sélectionnez Exécuter l’application de bureau Exécuter, tapez services.msc, puis appuyez sur Entrée. Faites défiler vers le bas jusqu’au service WebClient et assurez-vous que la colonne **État** affiche « En cours d’exécution ». Si ce n’est pas le cas, double-cliquez sur le service, cliquez sur **Démarrer,** puis sur **OK.** (Vous devrez peut-être d’abord  activer le service en sélectionnant Manuel ou Automatique **dans** la zone Type **de démarrage.)** 
    
> [!NOTE]
> L’ouverture d’une bibliothèque dans l’Explorateur de fichiers est pratique si vous devez copier ou déplacer plusieurs fichiers et dossiers une seule fois, mais si vous souhaitez travailler régulièrement dans la bibliothèque, nous vous recommandons de la synchroniser. Pour résoudre les problèmes d’ouverture dans l’Explorateur de fichiers, voir [Ouvrir dans l’Explorateur.](https://go.microsoft.com/fwlink/?linkid=871665) Pour plus d’informations sur la configuration de la synchronisation, [voir Synchroniser SharePoint fichiers avec le](https://go.microsoft.com/fwlink/?linkid=871666)nouveau client Synchronisation OneDrive.
  
Consultez l’article Sur l’utilisation de la commande « Ouvrir avec l’Explorateur » pour résoudre les problèmes dans [SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) pour plus d’informations. 
  

