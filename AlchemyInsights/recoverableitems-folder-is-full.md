---
title: 1336 le dossier RecoverableItems est plein
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741265"
---
# <a name="the-recoverable-items-folder-is-full"></a>Le dossier éléments récupérables est plein

Pour les boîtes aux lettres Exchange Online, la limite de stockage par défaut pour le dossier éléments récupérables est de 30 Go. La limite de stockage pour le dossier éléments récupérables est automatiquement augmentée à 100 Go si la boîte aux lettres est placée en conservation pour litige, conservation eDiscovery ou si elle est affectée à une stratégie de rétention.

Lorsque le dossier éléments récupérables atteint la limite de stockage, la fonctionnalité de boîte aux lettres est affectée des manières suivantes :

- L’utilisateur ne peut pas supprimer des éléments de la boîte aux lettres.

- L'Assistant Dossier géré ne peut pas supprimer des éléments en fonction de la balise de rétention ou des paramètres de dossiers gérés.

- Pour les boîtes aux lettres pour lesquelles la récupération d’élément unique est activée ou qui sont placées en conservation, le processus de protection de page de copie sur écriture ne peut pas conserver les versions des éléments modifiés par l’utilisateur.

- Pour les boîtes aux lettres pour lesquelles l’enregistrement d’audit de boîte aux lettres est activé, aucune entrée de journal d’audit de boîte aux lettres ne peut être enregistrée dans le sous-dossier audits du dossier éléments récupérables.

Pour les boîtes aux lettres qui ne sont pas en attente, les administrateurs peuvent utiliser la `Search-Mailbox -SearchDumpsterOnly -DeleteContent` commande dans Exchange Online PowerShell pour supprimer des éléments dans le dossier éléments récupérables. Pour plus d’informations, voir les rubriques suivantes :

- [Rechercher et supprimer des messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pour les boîtes aux lettres en attente, les administrateurs doivent supprimer le blocage avant de pouvoir supprimer des éléments du dossier éléments récupérables. Pour plus d’informations, consultez [la rubrique supprimer des éléments dans le dossier éléments récupérables des boîtes aux lettres en nuage en conservation](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Pour éviter que le dossier éléments récupérables ne devienne saturé, les administrateurs peuvent augmenter la limite de stockage du dossier éléments récupérables pour les boîtes aux lettres en attente et configurer une stratégie de rétention de boîte aux lettres qui déplace les éléments du dossier éléments récupérables vers la boîte aux lettres d’archivage de l’utilisateur. Voir [augmenter le quota des éléments récupérables pour les boîtes aux lettres en attente](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
