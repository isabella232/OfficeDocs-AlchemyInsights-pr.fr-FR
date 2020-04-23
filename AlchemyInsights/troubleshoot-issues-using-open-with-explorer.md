---
title: Résolution des problèmes à l’aide de la fonction ouvrir avec l’Explorateur
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759690"
---
# <a name="fix-problems-with-open-with-explorer"></a>Résoudre les problèmes liés à ouvrir avec l’Explorateur

Résoudre les problèmes courants liés à l’ouverture d’une bibliothèque de documents dans SharePoint ou OneDrive à l’aide de la commande **Ouvrir avec l’Explorateur** : 
  
- Utilisez Internet Explorer 10 ou Internet Explorer 11. **Open with Explorer** n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres. **Ouvrir avec l’Explorateur** est désactivé dans tous les navigateurs à l’exception d’Internet Explorer. 
    
- La **fonction ouvrir avec l’Explorateur** n’est pas disponible dans l’expérience moderne des bibliothèques SharePoint. Utilisez plutôt **l’affichage dans l’Explorateur de fichiers** . Sélectionnez View **options** \> **View dans l’Explorateur de fichiers**. L’affichage dans l’Explorateur de fichiers n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres. **Afficher dans l’Explorateur de fichiers** disponible uniquement dans Internet Explorer. 
    
- Assurez-vous que le service WebClient est en cours d’exécution. Dans la zone de recherche Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services. msc, puis appuyez sur entrée. Faites défiler jusqu’au service WebClient et assurez-vous que la colonne **État** affiche « en cours d’exécution ». Si ce n’est pas le cas, double-cliquez sur le service, cliquez sur **Démarrer**, puis cliquez sur **OK**. (Vous devrez peut-être activer d’abord le service en sélectionnant **Manuel** ou **automatique** dans la zone **type de démarrage** .) 
    
> [!NOTE]
> L’ouverture d’une bibliothèque dans l’Explorateur de fichiers est pratique si vous devez copier ou déplacer plusieurs fichiers et dossiers une seule fois, mais si vous souhaitez travailler régulièrement dans la bibliothèque, nous vous recommandons de la synchroniser. Pour résoudre les problèmes qui s’ouvrent dans l’Explorateur de fichiers, consultez la rubrique [ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665). Pour plus d’informations sur la configuration de la synchronisation, voir [synchroniser des fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Pour plus d’informations, reportez-vous à l’article [comment utiliser la commande « Ouvrir avec l’Explorateur » pour résoudre les problèmes dans SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

