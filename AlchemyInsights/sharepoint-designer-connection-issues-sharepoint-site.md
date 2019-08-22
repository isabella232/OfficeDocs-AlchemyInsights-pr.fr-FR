---
title: Problèmes de connexion avec SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508421"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="3ebf7-102">Problèmes de connexion avec SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="3ebf7-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="3ebf7-103">Si SharePoint Designer rencontre des problèmes de connexion aux sites SharePoint, essayez les solutions courantes suivantes.</span><span class="sxs-lookup"><span data-stu-id="3ebf7-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="3ebf7-104">Étape 1: Vérifiez que SharePoint Designer 2013 est mis à jour avec [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) et la [mise à jour 2016 du 2 août pour SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="3ebf7-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="3ebf7-105">Étape 2: effacez les fichiers du cache local:</span><span class="sxs-lookup"><span data-stu-id="3ebf7-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="3ebf7-106">Fermez SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3ebf7-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="3ebf7-107">Sur l’ordinateur local, supprimez tous les fichiers trouvés dans chacun des dossiers suivants.</span><span class="sxs-lookup"><span data-stu-id="3ebf7-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="3ebf7-108">%APPDATA%\Microsoft\Web serveur Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="3ebf7-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="3ebf7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="3ebf7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="3ebf7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="3ebf7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="3ebf7-111">Ouvrez SharePoint Designer 2013 et entrez à nouveau le compte pour voir s’il fonctionne.</span><span class="sxs-lookup"><span data-stu-id="3ebf7-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="3ebf7-112">Étape 3: [activez l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3ebf7-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="3ebf7-113">Étape 4: les administrateurs devront **autoriser les scripts personnalisés** dans les paramètres du centre d’administration SharePoint pour autoriser la connexion à SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="3ebf7-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="3ebf7-114">Pour plus d’informations, reportez-vous à la rubrique [autoriser ou empêcher un script personnalisé](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="3ebf7-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


