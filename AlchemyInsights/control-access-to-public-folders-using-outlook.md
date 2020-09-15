---
title: Contrôler l’accès aux dossiers publics à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680484"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Contrôler l’accès aux dossiers publics à l’aide d’Outlook

Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook :

1. Utiliser `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Remarque : Cette procédure peut uniquement contrôler les connexions avec les applications de bureau Outlook pour les clients Windows. Les utilisateurs ont toujours accès aux dossiers publics par le biais d’OWA ou d’Outlook pour Mac.

Pour plus d’informations, se référer à la rubrique [Connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).
