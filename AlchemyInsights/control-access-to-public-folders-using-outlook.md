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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816738"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Contrôler l’accès aux dossiers publics à l’aide d’Outlook

Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook :

1. Utiliser `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook  
$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook. Ceci est la valeur par défaut.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Remarque : Cette procédure peut uniquement contrôler les connexions avec les applications de bureau Outlook pour les clients Windows. Les utilisateurs ont toujours accès aux dossiers publics par le biais d’OWA ou d’Outlook pour Mac.

Pour plus d’informations, se référer à la rubrique [Connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).
