---
title: Restaurer un dossier public supprimé
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809437"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurer un dossier public supprimé

**Pour restaurer les éléments supprimés d'un dossier public**:

- See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).
 
**Pour restaurer un dossier public supprimé (de n'importe quel type)**: 

- Utilisez la commande EXO PowerShell suivante :

    Syntaxe :

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemple : la commande suivante restaure Subfolder1 et la place sous \Parent1 :

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pour [plus d'informations, voir](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Restaurer un dossier public supprimé.
