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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694454"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="f449b-102">Ouvrir avec l’Explorateur ne fonctionne pas</span><span class="sxs-lookup"><span data-stu-id="f449b-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="f449b-103">Si **Ouvrir avec l’Explorateur** ou **afficher dans l’Explorateur de fichiers** ne fonctionne pas, vérifiez que le service WebClient est configuré pour **s’exécuter** en suivant les étapes ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="f449b-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="f449b-104">Par exemple, l’ouverture d’une bibliothèque SharePoint ou OneDrive peut prendre beaucoup de temps lorsque le service n’est pas en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="f449b-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="f449b-105">Dans la zone de recherche Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services. msc, puis appuyez sur **entrée**.</span><span class="sxs-lookup"><span data-stu-id="f449b-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="f449b-106">Faites défiler vers le bas jusqu’au service WebClient et vérifiez la colonne **État** .</span><span class="sxs-lookup"><span data-stu-id="f449b-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="f449b-107">Si l’état du service WebClient n’est pas **en cours d’exécution**, double-cliquez sur le service, cliquez sur **Démarrer**, puis sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="f449b-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="f449b-108">Activez le service, le cas échéant, en sélectionnant **Manuel** ou **automatique** dans la zone **type de démarrage** .</span><span class="sxs-lookup"><span data-stu-id="f449b-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="f449b-109">Pour résoudre les problèmes qui s’ouvrent dans l’Explorateur de fichiers, consultez la rubrique [ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="f449b-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="f449b-110">Explorez la synchronisation en tant qu’alternative plus efficace : [synchroniser les fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="f449b-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

