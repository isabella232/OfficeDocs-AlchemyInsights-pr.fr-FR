---
title: Contrôler l’accès aux dossiers publics à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032556"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Contrôler l’accès aux dossiers publics à l’aide d’Outlook

Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook :

1. Utiliser `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Remarque : Cette procédure peut uniquement contrôler les connexions avec les applications de bureau Outlook pour les clients Windows. Les utilisateurs ont toujours accès aux dossiers publics par le biais d’OWA ou d’Outlook pour Mac.

Pour plus d’informations, se référer à la rubrique [Connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).
