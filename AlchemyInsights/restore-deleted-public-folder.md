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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943373"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurer un dossier public supprimé

**Pour restaurer les éléments supprimés d’un dossier public**:

- See [You can’t recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).
 
**Pour restaurer un dossier public supprimé (de n’importe quel type)**: 

- Utilisez la commande EXO PowerShell suivante :

    Syntaxe :

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemple : la commande suivante restaure Subfolder1 et la place sous \Parent1 :

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pour [plus d’informations, voir](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Restaurer un dossier public supprimé.
