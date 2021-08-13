---
title: Le dossier 1336 RecoverableItems est plein
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061754"
---
# <a name="the-recoverable-items-folder-is-full"></a>Le dossier Éléments récupérables est plein

Pour Exchange Online boîtes aux lettres, la limite de stockage par défaut pour le dossier Éléments récupérables est de 30 Go. La limite de stockage du dossier Éléments récupérables est automatiquement augmentée à 100 Go si la boîte aux lettres est placée en conservation pour litige, en conservation eDiscovery ou si elle est affectée à une stratégie de rétention.

Lorsque le dossier Éléments récupérables atteint la limite de stockage, la fonctionnalité de boîte aux lettres est affectée des manières suivantes :

- L’utilisateur ne peut pas supprimer d’éléments de la boîte aux lettres.

- L'Assistant Dossier géré ne peut pas supprimer des éléments en fonction de la balise de rétention ou des paramètres de dossiers gérés.

- Pour les boîtes aux lettres pour qui la récupération d’élément unique est activée ou qui sont placées en attente, le processus de protection de page de copie sur écriture ne peut pas gérer les versions des éléments modifiés par l’utilisateur.

- Pour les boîtes aux lettres pour qui l’enregistrement d’audit des boîtes aux lettres est activé, aucune entrée du journal d’audit de boîte aux lettres ne peut être enregistrée dans le sous-dossier Audits du dossier Éléments récupérables.

Pour les boîtes aux lettres qui ne sont pas en attente, les administrateurs peuvent utiliser la commande dans Exchange Online PowerShell pour supprimer des éléments dans le dossier `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Éléments récupérables. Pour plus d’informations, voir les rubriques suivantes :

- [Rechercher et supprimer des messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pour les boîtes aux lettres qui sont en attente, les administrateurs doivent supprimer la boîte aux lettres pour pouvoir supprimer des éléments du dossier Éléments récupérables. Pour plus d’informations, voir Supprimer des éléments dans le dossier [Éléments récupérables des](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)boîtes aux lettres en nuage en attente.

Pour éviter que le dossier Éléments récupérables ne devienne complet, les administrateurs peuvent augmenter la limite de stockage du dossier Éléments récupérables pour les boîtes aux lettres en attente et configurer une stratégie de rétention de boîte aux lettres qui déplace les éléments du dossier Éléments récupérables vers la boîte aux lettres d’archivage de l’utilisateur. Voir [Augmenter le quota d’éléments récupérables pour les boîtes aux lettres en attente.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
