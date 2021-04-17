---
title: Le propriétaire ne peut pas créer un sous-dossier à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836133"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Le propriétaire ne peut pas créer un sous-dossier à l’aide d’Outlook

**Il y a un problème permanent lié aux propriétaires de dossiers publics qui créent des sous-dossiers à l’aide d’Outlook. Le problème sera prochainement résolu.**

En attendant, vous pouvez utiliser l'une des solutions de contournement suivantes :

1. Utiliser Outlook pour MAC pour créer le sous-dossier en tant que problème concernant uniquement Outlook pour Windows (toutes les versions)
2. Demandez à l’administrateur de créer le sous-dossier à l’aide de EXO Shell ou EAC
3. Remplacez DefaultPublicFolderMailbox/EffectivePublicFolderMailbox de l’utilisateur par une autre boîte aux lettres que la boîte aux lettres de contenu pour le dossier à l’origine du problème.  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Patienter pendant une heure, redémarrez le client Outlook