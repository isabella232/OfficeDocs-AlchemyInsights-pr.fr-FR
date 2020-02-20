---
title: Pour un lot de migration de dossiers publics avec l’État CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158602"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pour un lot de migration de dossiers publics avec l’État CompletedWithErrors

Procédez comme suit pour terminer le lot, en ignorant les grands/mauvais éléments : 
1. Approuver les éléments ignorés sur le lot de migration :

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilisez la commande suivante pour approuver les éléments ignorés sur les demandes de migration qui sont « synchronisées » mais pas terminées :

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Le lot de migration et les demandes doivent reprendre et se terminer en quelques minutes.

