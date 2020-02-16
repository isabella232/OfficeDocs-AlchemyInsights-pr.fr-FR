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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043585"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pour un lot de migration de dossiers publics avec l’État CompletedWithErrors

Procédez comme suit pour terminer le lot, en ignorant les grands/mauvais éléments : 
1. Approuver les éléments ignorés sur le lot de migration :

    Set-MigrationBatch \<BatchName>-ApproveSkippedItems 
2. Utilisez la commande suivante pour approuver les éléments ignorés sur les demandes de migration qui sont « synchronisées » mais pas terminées :

    $pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport ; ForEach ($i dans $pf) {if ($i. LargeItemsEncountered-gt 0-ou $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime] :: UtcNow)}}
3. Le lot de migration et les demandes doivent reprendre et se terminer en quelques minutes.

