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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891747"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne peut pas se connecter aux dossiers publics

Si l’accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :

Connectez-vous à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d’utilisateur posant problème pour qu’il corresponde au paramètre sur un compte d’utilisateur de travail.

Exemple :

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valeur de la commande précédente>

Patientez au moins une heure pour que la modification prenne effet.

Si le problème persiste, suivez [cette procédure](https://aka.ms/pfcte) pour résoudre les problèmes d’accès aux dossiers publics à l’aide d’Outlook.