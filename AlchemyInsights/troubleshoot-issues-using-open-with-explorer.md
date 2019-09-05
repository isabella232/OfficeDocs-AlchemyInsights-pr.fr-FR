---
title: Résolution des problèmes à l’aide de la fonction ouvrir avec l’Explorateur
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742731"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="eb1e6-102">Résoudre les problèmes liés à ouvrir avec l’Explorateur</span><span class="sxs-lookup"><span data-stu-id="eb1e6-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="eb1e6-103">Résoudre les problèmes courants liés à l’ouverture d’une bibliothèque de documents dans SharePoint ou OneDrive à l’aide de la commande **Ouvrir avec l’Explorateur** :</span><span class="sxs-lookup"><span data-stu-id="eb1e6-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="eb1e6-104">Utilisez Internet Explorer 10 ou Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="eb1e6-105">**Open with Explorer** n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="eb1e6-106">**Ouvrir avec l’Explorateur** est désactivé dans tous les navigateurs à l’exception d’Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="eb1e6-107">La **fonction ouvrir avec l’Explorateur** n’est pas disponible dans l’expérience moderne des bibliothèques SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="eb1e6-108">Utilisez plutôt **l’affichage dans l’Explorateur de fichiers** .</span><span class="sxs-lookup"><span data-stu-id="eb1e6-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="eb1e6-109">Sélectionnez View **options** \> **View dans l’Explorateur de fichiers**.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="eb1e6-110">L’affichage dans l’Explorateur de fichiers n’est pas compatible avec Microsoft Edge, Google Chrome, Firefox et d’autres.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="eb1e6-111">**Afficher dans l’Explorateur de fichiers** disponible uniquement dans Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="eb1e6-112">Assurez-vous que le service WebClient est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="eb1e6-113">Dans la zone de recherche Windows, tapez exécuter, sélectionnez l’application de bureau exécuter, tapez services. msc, puis appuyez sur entrée.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="eb1e6-114">Faites défiler jusqu’au service WebClient et assurez-vous que la colonne **État** affiche « en cours d’exécution ».</span><span class="sxs-lookup"><span data-stu-id="eb1e6-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="eb1e6-115">Si ce n’est pas le cas, double-cliquez sur le service, cliquez sur **Démarrer**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="eb1e6-116">(Vous devrez peut-être activer d’abord le service en sélectionnant **Manuel** ou **automatique** dans la zone **type de démarrage** .)</span><span class="sxs-lookup"><span data-stu-id="eb1e6-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="eb1e6-117">L’ouverture d’une bibliothèque dans l’Explorateur de fichiers est pratique si vous devez copier ou déplacer plusieurs fichiers et dossiers une seule fois, mais si vous souhaitez travailler régulièrement dans la bibliothèque, nous vous recommandons de la synchroniser.</span><span class="sxs-lookup"><span data-stu-id="eb1e6-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="eb1e6-118">Pour résoudre les problèmes qui s’ouvrent dans l’Explorateur de fichiers, consultez la rubrique [ouvrir dans l’Explorateur](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="eb1e6-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="eb1e6-119">Pour plus d’informations sur la configuration de la synchronisation, voir [synchroniser des fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="eb1e6-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="eb1e6-120">Pour plus d’informations, reportez-vous à l’article [comment utiliser la commande « Ouvrir avec l’Explorateur » pour résoudre les problèmes dans SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="eb1e6-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

