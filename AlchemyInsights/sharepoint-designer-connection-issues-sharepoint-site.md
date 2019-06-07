---
title: Niveaux d’autorisation SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760691"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="19c6f-102">Problèmes de connexion avec SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="19c6f-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="19c6f-103">Si SharePoint Designer rencontre des problèmes de connexion aux sites SharePoint, essayez les solutions courantes suivantes.</span><span class="sxs-lookup"><span data-stu-id="19c6f-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="19c6f-104">Étape 1: Vérifiez que SharePoint Designer est mis à jour.</span><span class="sxs-lookup"><span data-stu-id="19c6f-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="19c6f-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="19c6f-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="19c6f-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="19c6f-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="19c6f-107">Mise à jour pour SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="19c6f-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="19c6f-108">Étape 2: effacer les fichiers du cache local</span><span class="sxs-lookup"><span data-stu-id="19c6f-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="19c6f-109">Fermez SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="19c6f-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="19c6f-110">Sur l’ordinateur local, accédez aux dossiers suivants pour supprimer les fichiers mis en cache.</span><span class="sxs-lookup"><span data-stu-id="19c6f-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="19c6f-111">Cliquez sur Démarrer, exécutez et supprimez tous les fichiers trouvés sous chacun des emplacements ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="19c6f-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="19c6f-112">%APPDATA%\Microsoft\Web Server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="19c6f-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="19c6f-113">Ouvrez SharePoint Designer 2013 et entrez à nouveau le compte pour voir s’il fonctionne.</span><span class="sxs-lookup"><span data-stu-id="19c6f-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="19c6f-114">Étape 3: [activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="19c6f-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="19c6f-115">Étape 4: les administrateurs devront autoriser le script personnalisé à autoriser la connexion à SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="19c6f-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="19c6f-116">Pour obtenir la procédure détaillée, des exemples et des considérations, voir [autoriser ou empêcher les scripts personnalisés](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="19c6f-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


