---
title: 1336 le dossier RecoverableItems est plein
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 8a5859ba29d847606e8b44d169c3cd6a26364744
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36509733"
---
# <a name="the-recoverable-items-folder-is-full"></a>Le dossier éléments récupérables est plein

Pour les boîtes aux lettres Exchange Online dans Office 365, la limite de stockage par défaut pour le dossier éléments récupérables est de 30 Go. La limite de stockage pour le dossier éléments récupérables est automatiquement augmentée à 100 Go si la boîte aux lettres est placée en conservation pour litige, conservation eDiscovery ou est affectée à une stratégie de rétention Office 365.

Lorsque le dossier éléments récupérables atteint la limite de stockage, la fonctionnalité de boîte aux lettres est affectée des manières suivantes:

- L’utilisateur ne peut pas supprimer des éléments de la boîte aux lettres.

- L'Assistant Dossier géré ne peut pas supprimer des éléments en fonction de la balise de rétention ou des paramètres de dossiers gérés.

- Pour les boîtes aux lettres pour lesquelles la récupération d’élément unique est activée ou qui sont placées en conservation, le processus de protection de page de copie sur écriture ne peut pas conserver les versions des éléments modifiés par l’utilisateur.

- Pour les boîtes aux lettres pour lesquelles l’enregistrement d’audit de boîte aux lettres est activé, aucune entrée de journal d’audit de boîte aux lettres ne peut être enregistrée dans le sous-dossier audits du dossier éléments récupérables.

Pour les boîtes aux lettres qui ne sont pas en attente, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` les administrateurs peuvent utiliser la commande dans Exchange Online PowerShell pour supprimer des éléments dans le dossier éléments récupérables. Pour plus d’informations, consultez les rubriques suivantes :

- [Rechercher et supprimer des messages](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pour les boîtes aux lettres en attente, les administrateurs doivent supprimer le blocage avant de pouvoir supprimer des éléments du dossier éléments récupérables. Pour plus d’informations, consultez [la rubrique supprimer des éléments dans le dossier éléments récupérables des boîtes aux lettres en nuage en conservation](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Pour éviter que le dossier éléments récupérables ne devienne saturé, les administrateurs peuvent augmenter la limite de stockage du dossier éléments récupérables pour les boîtes aux lettres en conservation et configurer une stratégie de rétention de boîte aux lettres qui déplace les éléments du dossier éléments récupérables vers l’archive de l’utilisateur. lettres. Voir [augmenter le quota des éléments récupérables pour les boîtes aux lettres en attente](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
