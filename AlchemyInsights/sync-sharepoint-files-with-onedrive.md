---
title: Résoudre les problèmes « Ouvrir avec l’Explorateur » dans SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086046"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="95ed0-102">Résoudre les problèmes « Ouvrir avec l’Explorateur » dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="95ed0-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="95ed0-103">Suivez les étapes et pratiques recommandées dans les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="95ed0-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="95ed0-104">Utiliser la commande « Ouvrir avec l’Explorateur » pour résoudre des problèmes dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="95ed0-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="95ed0-105">Copier ou déplacer des fichiers de bibliothèque à l’aide de la commande Ouvrir avec Explorateur</span><span class="sxs-lookup"><span data-stu-id="95ed0-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="95ed0-106">Nous vous recommandons de [synchroniser les fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) qui offre Des [fichiers à la demande](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) en fournit un accès local à vos fichiers et offre de meilleures performances.</span><span class="sxs-lookup"><span data-stu-id="95ed0-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="95ed0-107">**L’ouverture avec l’Explorateur** est prise en charge uniquement dans Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="95ed0-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="95ed0-108">Pour plus d’informations, consultez [fin du support pour IE11 avec les applications Microsoft 365](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span><span class="sxs-lookup"><span data-stu-id="95ed0-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="95ed0-109">**Ouvrir dans Explorer** ne fonctionne pas dans Windows avec Microsoft Edge, Google Chrome, Mozilla Firefox ou sur la plateforme Mac.</span><span class="sxs-lookup"><span data-stu-id="95ed0-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="95ed0-110">Pour cette raison, il est possible que l’option **Mode Explorateur** soit grisée.</span><span class="sxs-lookup"><span data-stu-id="95ed0-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="95ed0-111">Le bouton **Ouvrir avec l’Explorateur** ne s’affiche pas dans la nouvelle expérience de bibliothèque.</span><span class="sxs-lookup"><span data-stu-id="95ed0-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="95ed0-112">Sélectionnez la liste déroulante **Affichage** dans l’angle supérieur droit (le nom de la liste déroulante change en fonction de votre affichage actuel), puis cliquez sur **Afficher dans l’Explorateur de fichiers**.</span><span class="sxs-lookup"><span data-stu-id="95ed0-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

