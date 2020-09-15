---
title: Le propriétaire ne peut pas créer un sous-dossier à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665716"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Le propriétaire ne peut pas créer un sous-dossier à l’aide d’Outlook

**Il y a un problème permanent lié aux propriétaires de dossiers publics qui créent des sous-dossiers à l’aide d’Outlook. Le problème sera prochainement résolu.**

En attendant, vous pouvez utiliser l'une des solutions de contournement suivantes :

1. Utiliser Outlook pour MAC pour créer le sous-dossier en tant que problème concernant uniquement Outlook pour Windows (toutes les versions)
2. Demandez à l’administrateur de créer le sous-dossier à l’aide de EXO Shell ou EAC
3. Remplacez DefaultPublicFolderMailbox/EffectivePublicFolderMailbox de l’utilisateur par une autre boîte aux lettres que la boîte aux lettres de contenu pour le dossier à l’origine du problème.  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Patienter pendant une heure, redémarrez le client Outlook