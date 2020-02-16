---
title: Restaurer un dossier public supprimé
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063646"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="83c97-102">Restaurer un dossier public supprimé</span><span class="sxs-lookup"><span data-stu-id="83c97-102">Restore a deleted public folder</span></span>

<span data-ttu-id="83c97-103">**Pour restaurer des éléments supprimés à partir d’un dossier public**:</span><span class="sxs-lookup"><span data-stu-id="83c97-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="83c97-104">Consultez [la rubrique vous ne pouvez pas récupérer les éléments supprimés à partir d’un dossier public non destiné à la messagerie dans Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="83c97-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="83c97-105">**Pour restaurer un dossier public supprimé (de n’importe quel type)**:</span><span class="sxs-lookup"><span data-stu-id="83c97-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="83c97-106">Utilisez la commande EXO PowerShell suivante :</span><span class="sxs-lookup"><span data-stu-id="83c97-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="83c97-107">Syntaxe :</span><span class="sxs-lookup"><span data-stu-id="83c97-107">Syntax:</span></span>

    ><span data-ttu-id="83c97-108">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse | ? {$_. Name-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity- \<Path chemin d’accès où le dossier sera restauré></span><span class="sxs-lookup"><span data-stu-id="83c97-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="83c97-109">Exemple : la commande suivante permet de restaurer Subfolder1 et de le placer sous \Parent1 :</span><span class="sxs-lookup"><span data-stu-id="83c97-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="83c97-110">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse | ? {$_. Name-EQ "Subfolder1"}; Set-PublicFolder $pf. Identity-Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="83c97-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="83c97-111">Pour plus d’informations, reportez-vous à [la rubrique restaurer un dossier public supprimé](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="83c97-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
