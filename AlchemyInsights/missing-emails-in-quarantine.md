---
title: Messages manquants en quarantaine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542152"
---
# <a name="missing-emails-in-quarantine"></a>Messages manquants en quarantaine

Les administrateurs peuvent [afficher, publier ou supprimer ces messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pour ouvrir le centre de sécurité & conformité, accédez à [https://protection.office.com](https://protection.office.com/) . Pour ouvrir la page de mise en quarantaine directement, accédez à [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Vous pouvez effectuer une recherche sur les valeurs suivantes :  

- **ID du message** : l’identificateur global unique du message. Si vous sélectionnez un message dans la liste, la valeur de l' **ID du message** s’affiche dans le volet flyout de **Détails** qui s’affiche. Les administrateurs peuvent utiliser le [suivi des messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pour rechercher les messages et les valeurs d’ID de message correspondantes.
- **Adresse e-mail de l'expéditeur** : adresse e-mail d'un seul expéditeur.
- **Adresse e-mail du destinataire** : adresse e-mail d'un seul destinataire.
- **Sujet** : utiliser l'intégralité du sujet du message. La recherche n’est pas sensible à la casse.

Une fois que vous avez entré les critères de recherche, cliquez sur Actualiser ![ le bouton ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualiser** pour filtrer les résultats.  

Les cmdlets que vous utilisez pour afficher et gérer les messages et les fichiers en quarantaine sont les suivantes :
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Notez que cette applet de commande concerne uniquement les messages, pas les fichiers de programmes malveillants, pour SharePoint Online, OneDrive entreprise ou Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)