---
title: Blocage du téléchargement via des liens de partage
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685740"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="7a8e8-102">Blocage du téléchargement via des liens de partage</span><span class="sxs-lookup"><span data-stu-id="7a8e8-102">Block download on sharing links</span></span>

<span data-ttu-id="7a8e8-103">**Bloquer le téléchargement** est disponible pour les **liens en affichage seul** vers les documents Office.</span><span class="sxs-lookup"><span data-stu-id="7a8e8-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="7a8e8-104">Lorsque vous sélectionnez cette option, les personnes qui accèdent au fichier via le lien que vous avez créé ne voient pas les options de téléchargement, d’impression ni de copie du fichier.</span><span class="sxs-lookup"><span data-stu-id="7a8e8-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="7a8e8-105">Les administrateurs peuvent contrôler si le paramètre Bloquer le téléchargement s’affiche uniquement pour les fichiers Office ou non en modifiant le paramètre de `BlockDownloadLinksFileType` dans les cmdlets PowerShell [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) ou [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="7a8e8-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
