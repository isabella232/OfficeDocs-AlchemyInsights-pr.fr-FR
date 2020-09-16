---
title: Pour un lot de migration de dossiers publics avec l’État CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744111"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="005b6-102">Pour un lot de migration de dossiers publics avec l’État CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="005b6-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="005b6-103">Procédez comme suit pour terminer le lot, en ignorant les grands/mauvais éléments :</span><span class="sxs-lookup"><span data-stu-id="005b6-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="005b6-104">Approuver les éléments ignorés sur le lot de migration :</span><span class="sxs-lookup"><span data-stu-id="005b6-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="005b6-105">Utilisez la commande suivante pour approuver les éléments ignorés sur les demandes de migration qui sont « synchronisées » mais pas terminées :</span><span class="sxs-lookup"><span data-stu-id="005b6-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="005b6-106">Le lot de migration et les demandes doivent reprendre et se terminer en quelques minutes.</span><span class="sxs-lookup"><span data-stu-id="005b6-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

