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
# <a name="restore-a-deleted-public-folder"></a>Restaurer un dossier public supprimé

**Pour restaurer des éléments supprimés à partir d’un dossier public**:

- Consultez [la rubrique vous ne pouvez pas récupérer les éléments supprimés à partir d’un dossier public non destiné à la messagerie dans Outlook 2016](https://aka.ms/pfrec).
 
**Pour restaurer un dossier public supprimé (de n’importe quel type)**: 

- Utilisez la commande EXO PowerShell suivante :

    Syntaxe :

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse | ? {$_. Name-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity- \<Path chemin d’accès où le dossier sera restauré>

    Exemple : la commande suivante permet de restaurer Subfolder1 et de le placer sous \Parent1 :

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse | ? {$_. Name-EQ "Subfolder1"}; Set-PublicFolder $pf. Identity-Path \Parent1

Pour plus d’informations, reportez-vous à [la rubrique restaurer un dossier public supprimé](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
