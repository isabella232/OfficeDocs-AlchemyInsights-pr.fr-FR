---
title: Messages électroniques manquants en quarantaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539822"
---
# <a name="missing-emails-in-quarantine"></a>Messages électroniques manquants en quarantaine »

Les administrateurs [peuvent afficher, libérer ou supprimer ces messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Pour ouvrir le Centre de sécurité & conformité, allez dans [https://protection.office.com](https://protection.office.com/) . Pour ouvrir la page de mise en quarantaine directement, allez sur [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Vous pouvez effectuer une recherche sur les valeurs suivantes :  

- **ID du message** : l’identificateur global unique du message. Si vous sélectionnez un message dans la liste, la valeur  **de l’ID**  de message apparaît dans le volet volant  **Détails**  qui s’affiche. Les administrateurs peuvent utiliser le [suivi des messages](/microsoft-365/security/office-365-security/message-trace-scc) pour rechercher les messages et les valeurs d’ID de message correspondantes.
- **Adresse e-mail de l'expéditeur** : adresse e-mail d'un seul expéditeur.
- **Adresse e-mail du destinataire** : adresse e-mail d'un seul destinataire.
- **Sujet** : utiliser l'intégralité du sujet du message. La recherche n’est pas sensible à la casse.

Après avoir entrer les critères de recherche, cliquez sur le ![Bouton actualiser](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualiser** pour filtrer les résultats.

Les cmdlets que vous utilisez pour afficher et gérer les messages et les fichiers en quarantaine sont :
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): notez que cette cmdlet est uniquement pour les messages, et non pour les fichiers de programmes malveillants de Microsoft Defender pour Office 365 pour SharePoint Online, OneDrive Entreprise ou Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)