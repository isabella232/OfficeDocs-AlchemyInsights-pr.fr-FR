---
title: Pour le lot de migration de dossiers publics avec l’état CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068162"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pour le lot de migration de dossiers publics avec l’état CompletedWithErrors

Utilisez les étapes suivantes pour terminer le lot, en ignorer les éléments grands/mauvais : 
1. Approuvez les éléments ignorés sur le lot de migration :

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilisez la commande suivante pour approuver les éléments ignorés sur les demandes de migration qui sont « synchronisées », mais qui ne sont pas terminées :

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Le lot de migration et les demandes doivent reprendre et se terminer dans quelques minutes.

