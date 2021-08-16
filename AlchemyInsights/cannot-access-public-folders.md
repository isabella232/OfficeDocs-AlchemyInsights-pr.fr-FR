---
title: Impossible d’accéder aux dossiers publics
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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996628"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne peut pas se connecter aux dossiers publics

Si l’accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :

Connecter à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d’utilisateur problème pour qu’il corresponde au paramètre sur un compte d’utilisateur de travail.

Exemple :

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Attendez au moins une heure que la modification prenne effet.

Si le problème demeure, suivez cette procédure pour [résoudre](https://aka.ms/pfcte) les problèmes d’accès aux dossiers publics à l’aide Outlook.
 
**Pour contrôler les utilisateurs qui peuvent accéder aux dossiers publics à l’aide Outlook**:

1.  Utiliser Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
      
    $false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Remarque** Cette procédure ne peut contrôler les connexions qu’avec Outlook bureau pour Windows clients. Un utilisateur peut continuer à accéder aux dossiers publics à l’aide OWA ou Outlook pour Mac.
 
Pour plus d’informations, voir Annonce de la prise en charge des [connexions contrôlées](https://aka.ms/controlpf)aux dossiers publics dans Outlook .