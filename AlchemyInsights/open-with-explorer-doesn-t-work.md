---
title: Ouvrir avec l’Explorateur ne fonctionne pas
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
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538467"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8ad35-102">Ouvrir avec l’Explorateur ne fonctionne pas</span><span class="sxs-lookup"><span data-stu-id="8ad35-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8ad35-103">Si **Ouvrir avec l’Explorateur** ou **afficher dans l’Explorateur de fichiers** ne fonctionne pas, vérifiez que le service WebClient est configuré pour **s’exécuter** en suivant les étapes ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8ad35-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8ad35-104">Par exemple, l’ouverture d’une bibliothèque SharePoint ou OneDrive peut prendre beaucoup de temps lorsque le service n’est pas en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="8ad35-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8ad35-105">Dans la zone de recherche Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services. msc, puis appuyez sur **entrée**.</span><span class="sxs-lookup"><span data-stu-id="8ad35-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8ad35-106">Faites défiler vers le bas jusqu’au service WebClient et vérifiez la colonne **État** .</span><span class="sxs-lookup"><span data-stu-id="8ad35-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8ad35-107">Si l’état du service WebClient n’est pas **en cours d’exécution**, double-cliquez sur le service, cliquez sur **Démarrer**, puis sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="8ad35-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8ad35-108">Activez le service, le cas échéant, en sélectionnant **Manuel** ou **automatique** dans la zone **type de démarrage** .</span><span class="sxs-lookup"><span data-stu-id="8ad35-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8ad35-109">Pour résoudre les problèmes qui s’ouvrent dans l’Explorateur de fichiers, consultez la rubrique [ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8ad35-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8ad35-110">Explorez la synchronisation en tant qu’alternative plus efficace: [synchroniser les fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8ad35-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

