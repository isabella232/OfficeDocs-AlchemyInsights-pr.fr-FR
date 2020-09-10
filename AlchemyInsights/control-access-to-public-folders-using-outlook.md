---
title: Contrôler l’accès aux dossiers publics à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406561"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Contrôler l’accès aux dossiers publics à l’aide d’Outlook

Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook :

1. Utiliser `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Remarque : Cette procédure peut uniquement contrôler les connexions avec les applications de bureau Outlook pour les clients Windows. Les utilisateurs ont toujours accès aux dossiers publics par le biais d’OWA ou d’Outlook pour Mac.

Pour plus d’informations, se référer à la rubrique [Connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).
