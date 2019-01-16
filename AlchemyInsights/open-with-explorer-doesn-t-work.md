---
title: Ouvrir dans l’Explorateur de solutions ne fonctionne pas
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287669"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="915a7-102">Ouvrir dans l’Explorateur de solutions ne fonctionne pas</span><span class="sxs-lookup"><span data-stu-id="915a7-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="915a7-p101">Si **Ouvrir avec l’Explorateur** ou **affichage dans l’Explorateur de fichiers** ne fonctionne pas, assurez-vous que le service WebClient est en cours **d’exécution** en suivant les étapes ci-dessous. Par exemple, il peut prendre beaucoup de temps pour ouvrir une bibliothèque SharePoint ou OneDrive lorsque le service n’est pas en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="915a7-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="915a7-105">Dans la zone de recherche de Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services.msc et puis sélectionnez **entrée**.</span><span class="sxs-lookup"><span data-stu-id="915a7-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="915a7-p102">Faites défiler jusqu'à la service WebClient et vérifiez la colonne **état** . Si l’état du service WebClient n’est pas **en cours d’exécution**, double-cliquez sur le service, cliquez sur **Démarrer**, puis cliquez sur **OK**. Activez le service, le cas échéant, en sélectionnant l’option **manuel** ou **automatique** dans la zone **type de démarrage** .</span><span class="sxs-lookup"><span data-stu-id="915a7-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="915a7-p103">Pour résoudre les problèmes d’ouverture dans l’Explorateur de fichiers, voir [Ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665). Explorez la synchronisation comme une meilleure solution : [fichiers de synchronisation SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="915a7-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

