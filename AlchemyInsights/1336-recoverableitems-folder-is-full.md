---
title: Le dossier RecoverableItems 1336 est plein
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909286"
---
# <a name="the-recoverable-items-folder-is-full"></a>Le dossier éléments récupérables est plein

Pour les boîtes aux lettres Exchange Online dans Office 365, la limite de stockage par défaut pour le dossier éléments récupérables est de 30 Go. La limite de stockage pour le dossier éléments récupérables est automatiquement augmentée à 100 Go si la boîte aux lettres est placé en blocage pour litige, blocage eDiscovery, ou est affecté à une stratégie de rétention d’Office 365.
  
Lorsque le dossier éléments récupérables atteint la limite de stockage, les fonctionnalités de boîte aux lettres sont affectée de la manière suivante :
  
- L’utilisateur ne peut pas supprimer des éléments dans la boîte aux lettres.
    
- L'Assistant Dossier géré ne peut pas supprimer des éléments en fonction de la balise de rétention ou des paramètres de dossiers gérés.
    
- Pour les boîtes aux lettres de récupération d’élément unique ou sont mis en attente, le processus de protection de page de la copie sur écriture ne peut pas mettre à jour les versions des éléments modifiés par l’utilisateur.
    
- Pour les boîtes aux lettres dont les boîtes aux lettres d’audit de l’enregistrement est activé, aucune entrée du journal d’audit boîte aux lettres ne peut être enregistrées dans le sous-dossier des Audits dans le dossier éléments récupérables.
    
Pour les boîtes aux lettres qui ne sont pas en attente, les administrateurs peuvent utiliser le `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command dans Exchange Online PowerShell pour supprimer des éléments dans le dossier éléments récupérables. Pour plus d’informations, voir les rubriques suivantes : 
  
- [Rechercher et supprimer des messages](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Pour les boîtes aux lettres qui sont en attente, administrateurs doivent retirer le blocage avant de pouvoir les éléments supprimés du dossier éléments récupérables. Pour plus d’informations, voir [Supprimer des éléments dans les éléments récupérables dossier de boîtes aux lettres en nuage sur contenir](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Pour vous aider à empêcher la saturation du dossier éléments récupérables, administrateurs peuvent augmenter la limite de stockage des éléments récupérables dossier pour les boîtes aux lettres sur Maintenez et définir une stratégie de rétention de boîte aux lettres qui déplace les éléments à partir du dossier éléments récupérables pour l’archivage de l’utilisateur boîte aux lettres. Voir [augmenter les éléments récupérables quota de boîtes aux lettres sur Maintenez](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

