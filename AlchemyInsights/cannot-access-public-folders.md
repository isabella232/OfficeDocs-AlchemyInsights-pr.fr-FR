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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959493"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne peut pas se connecter aux dossiers publics

Si l’accès aux dossiers publics ne fonctionne pas pour quelques utilisateurs, procédez comme suit :

Connectez-vous à EXO PowerShell et configurez le DefaultPublicFolderMailbox sur le compte d’utilisateur posant problème pour qu’il corresponde à un compte d’utilisateur en cours d’utilisation.

Exemple :

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valeur de la commande précédente>

Patientez au moins une heure pour que la modification prenne effet.