---
title: Impossible d'accéder aux dossiers publics
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
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819510"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne peut pas se connecter aux dossiers publics

Si l'accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :

Connectez-vous à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d'utilisateur à problème pour qu'il corresponde au paramètre sur un compte d'utilisateur de travail.

Exemple :

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Attendez au moins une heure que la modification prenne effet.

Si le problème demeure, suivez cette procédure pour [résoudre](https://aka.ms/pfcte) les problèmes d'accès aux dossiers publics à l'aide d'Outlook.
 
**Pour contrôler les utilisateurs qui peuvent accéder aux dossiers publics à l'aide d'Outlook**:

1.  Utiliser Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
      
    $false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Remarque** Cette procédure ne peut contrôler les connexions qu'avec les clients de bureau Outlook pour les clients Windows. Un utilisateur peut continuer à accéder aux dossiers publics à l'OWA ou Outlook pour Mac.
 
Pour plus d'informations, voir Annonce de la prise en [charge des connexions contrôlées aux dossiers publics dans Outlook.](https://aka.ms/controlpf)