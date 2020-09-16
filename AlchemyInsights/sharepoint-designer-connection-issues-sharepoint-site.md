---
title: Problèmes de connexion avec SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727169"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="dc9df-102">Problèmes de connexion avec SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="dc9df-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="dc9df-103">Si SharePoint Designer rencontre des problèmes de connexion aux sites SharePoint, essayez les solutions courantes suivantes.</span><span class="sxs-lookup"><span data-stu-id="dc9df-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="dc9df-104">Étape 1 : Vérifiez que SharePoint Designer 2013 est mis à jour avec [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) et la [mise à jour 2016 du 2 août pour SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="dc9df-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="dc9df-105">Étape 2 : effacez les fichiers du cache local :</span><span class="sxs-lookup"><span data-stu-id="dc9df-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="dc9df-106">Fermez SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="dc9df-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="dc9df-107">Sur l’ordinateur local, supprimez tous les fichiers trouvés dans chacun des dossiers suivants.</span><span class="sxs-lookup"><span data-stu-id="dc9df-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="dc9df-108">%APPDATA%\Microsoft\Web serveur Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="dc9df-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="dc9df-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="dc9df-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="dc9df-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="dc9df-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="dc9df-111">Ouvrez SharePoint Designer 2013 et entrez à nouveau le compte pour voir s’il fonctionne.</span><span class="sxs-lookup"><span data-stu-id="dc9df-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="dc9df-112">Étape 3 : [activez l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="dc9df-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="dc9df-113">Étape 4 : les administrateurs devront **autoriser les scripts personnalisés** dans les paramètres du centre d’administration SharePoint pour autoriser la connexion à SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="dc9df-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="dc9df-114">Pour plus d’informations, reportez-vous à la rubrique [autoriser ou empêcher un script personnalisé](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="dc9df-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


