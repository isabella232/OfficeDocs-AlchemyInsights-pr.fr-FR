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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158498"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurer un dossier public supprimé

**Pour restaurer des éléments supprimés à partir d’un dossier public**:

- Consultez [la rubrique vous ne pouvez pas récupérer les éléments supprimés à partir d’un dossier public non destiné à la messagerie dans Outlook 2016](https://aka.ms/pfrec).
 
**Pour restaurer un dossier public supprimé (de n’importe quel type)**: 

- Utilisez la commande EXO PowerShell suivante :

    Syntaxe :

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemple : la commande suivante permet de restaurer Subfolder1 et de le placer sous \Parent1 :

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pour plus d’informations, reportez-vous à [la rubrique restaurer un dossier public supprimé](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
