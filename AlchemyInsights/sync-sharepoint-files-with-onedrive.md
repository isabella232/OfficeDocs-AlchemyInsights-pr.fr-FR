---
title: Résoudre les problèmes « Ouvrir avec l’Explorateur » dans SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: fcaca189741bd68878b1dcfab879e6e0f64e6794
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223638"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="2c0b2-102">Résoudre les problèmes « Ouvrir avec l’Explorateur » dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2c0b2-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="2c0b2-103">La commande Ouvrir avec l’Explorateur ouvre une instance locale de l’Explorateur Windows qui affiche la structure de dossiers sur le serveur qui héberge le site SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="2c0b2-104">Cela dit, nous vous recommandons de [synchroniser les fichiers SharePoint avec le nouveau client de synchronisation OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> qui offre les [fichiers à la demande](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) en assurant l’accès local à vos fichiers et les meilleures performances.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="2c0b2-105">Si vous avez choisi d’utiliser le mode explorateur au lieu d’utiliser le nouveau client de synchronisation, veillez à suivre les étapes et les pratiques décrites dans les articles suivants.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="2c0b2-106">Utiliser la commande « Ouvrir avec l’Explorateur » pour résoudre des problèmes dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2c0b2-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="2c0b2-107">Copier ou déplacer des fichiers de bibliothèque à l’aide de la commande Ouvrir avec l’Explorateur</span><span class="sxs-lookup"><span data-stu-id="2c0b2-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="2c0b2-108">Remarque : le bouton Ouvrir avec l’Explorateur ne s’affiche pas dans la nouvelle expérience de bibliothèque.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="2c0b2-109">Cliquez sur la liste déroulante Affichage dans l’angle supérieur droit (le nom de la liste déroulante change en fonction de votre affichage actuel), puis cliquez sur Afficher dans l’Explorateur de fichiers.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="2c0b2-110">Ouvrir avec l’Explorateur dans SharePoint utilise des contrôles ActiveX. Il n’est donc pris en charge que dans Internet Explorer 10 ou 11.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="2c0b2-111">Ouvrir avec l’Explorateur ne fonctionne pas dans Windows avec Microsoft Edge, Google Chrome, Mozilla Firefox ni sur la plateforme Mac.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="2c0b2-112">Pour cette raison, il est possible que l’option Mode Explorateur soit grisée.</span><span class="sxs-lookup"><span data-stu-id="2c0b2-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="2c0b2-113">[Pourquoi des boutons du ruban SharePoint sont indisponibles ou grisés](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="2c0b2-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

