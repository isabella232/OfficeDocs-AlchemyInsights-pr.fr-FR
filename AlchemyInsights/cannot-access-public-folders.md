---
title: Impossible d’accéder aux dossiers publics
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
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341401"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne peut pas se connecter aux dossiers publics

Si l’accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :

Connectez-vous à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d’utilisateur posant problème pour qu’il corresponde au paramètre sur un compte d’utilisateur de travail.

Exemple :

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Patientez au moins une heure pour que la modification prenne effet.

Si le problème persiste, suivez [cette procédure](https://aka.ms/pfcte) pour résoudre les problèmes d’accès aux dossiers publics à l’aide d’Outlook.
 
**Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook**:

1.  Utilisation de Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true : autoriser les utilisateurs à accéder aux dossiers publics dans Outlook  
      
    $false : empêcher les utilisateurs d’accéder aux dossiers publics dans Outlook. Il s’agit de la valeur par défaut.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Note** Cette procédure permet de contrôler les connexions uniquement avec les clients Outlook pour ordinateur de bureau pour Windows. Un utilisateur peut continuer à accéder aux dossiers publics à l’aide d’OWA ou d’Outlook pour Mac.
 
Pour plus d’informations, consultez la rubrique [annonce de la prise en charge des connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).