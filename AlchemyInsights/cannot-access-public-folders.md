---
title: Impossible d’accéder aux dossiers publics
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
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812545"
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
      
    $true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
      
    $false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Note** Cette procédure permet de contrôler les connexions uniquement avec les clients Outlook pour ordinateur de bureau pour Windows. Un utilisateur peut continuer à accéder aux dossiers publics à l’aide d’OWA ou d’Outlook pour Mac.
 
Pour plus d’informations, consultez la rubrique [annonce de la prise en charge des connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).