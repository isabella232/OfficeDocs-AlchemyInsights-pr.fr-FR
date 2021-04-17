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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831732"
---
# <a name="missing-emails-in-quarantine"></a>Messages électroniques manquants en quarantaine »

Les administrateurs [peuvent afficher, libérer ou supprimer ces messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pour ouvrir le Centre de sécurité & conformité, allez dans [https://protection.office.com](https://protection.office.com/) . Pour ouvrir la page de mise en quarantaine directement, allez sur [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Vous pouvez effectuer une recherche sur les valeurs suivantes :  

- **ID du message** : l’identificateur global unique du message. Si vous sélectionnez un message dans la liste, la valeur  **de l'ID**  de message apparaît dans le volet volant  **Détails**  qui s'affiche. Les administrateurs peuvent utiliser le [suivi des messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pour rechercher les messages et les valeurs d’ID de message correspondantes.
- **Adresse e-mail de l'expéditeur** : adresse e-mail d'un seul expéditeur.
- **Adresse e-mail du destinataire** : adresse e-mail d'un seul destinataire.
- **Sujet** : utiliser l'intégralité du sujet du message. La recherche n’est pas sensible à la casse.

Une fois que vous avez entré les critères de recherche, cliquez sur Actualiser le bouton ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualiser** pour filtrer les résultats.  

Les cmdlets que vous utilisez pour afficher et gérer les messages et les fichiers en quarantaine sont :
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): notez que cette cmdlet est uniquement pour les messages, et non pour les fichiers de programmes malveillants de la protection anti-programme malveillant pour SharePoint Online, OneDrive Entreprise ou Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)