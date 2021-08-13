---
title: Outlook Rappel de bureau ou remplacement d’un message électronique
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918393"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Rappeler ou remplacer un message Outlook message électronique

- En tant qu’administrateur, vous pouvez rappeler des messages au nom des utilisateurs à **l’aide de PowerShell.** Vous ne pouvez pas rappeler les messages du Centre d’administration.
- Vous pouvez **uniquement rappeler les messages envoyés à des personnes de votre organisation.** Si le message a été envoyé à une adresse Gmail, par exemple, vous ne pouvez pas le rappeler.
- Vous ne pouvez **rappeler que les messages envoyés Outlook 2016 sur le PC.** Si un utilisateur envoie un message à l’Outlook pour Mac ou Outlook sur le web, vous ne pouvez pas le rappeler.

Pour rappeler ou remplacer un message électronique :

1. Dans le volet de dossiers à gauche de la fenêtre Outlook, sélectionnez le dossier Éléments envoyés.
1. Double-cliquez sur le message à rappeler pour l’ouvrir.
1. Sélectionnez **l’onglet Message,** puis **sélectionnez Actions**  >  **rappeler ce message.**
1. Sélectionnez **Supprimer les copies** non lues de ce message ou Supprimer les copies non lues et remplacer par un **nouveau message,** puis sélectionnez **OK**.
1. Si vous envoyez un message de remplacement, composez-le, puis sélectionnez **Envoyer.**
1. La réussite ou l’échec d’un rappel de message dépend des paramètres du destinataire Outlook. Pour savoir comment vérifier le rappel, consultez [cet article.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Recherche et suppression de messages électroniques dans votre organisation

- Si vous n’êtes pas un administrateur général, votre compte doit être ajouté au rôle gestionnaire eDiscovery ou au rôle de gestion de la recherche de conformité pour rechercher des messages. Pour supprimer des messages, vous devez rejoindre le groupe de rôles Gestion de l’organisation ou le rôle de gestion recherche et purge. Les autorisations pour ces rôles sont attribuées dans le Centre de sécurité [et conformité.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Créez une recherche de](https://docs.microsoft.com/microsoft-365/compliance/content-search) contenu pour rechercher le message à supprimer.
- [Connecter centre de sécurité et conformité PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Si vous utilisez l’authentification multifacteur, voir Connecter pour Microsoft 365 sécurité et conformité PowerShell à l’aide de [l’authentification multifacteur.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)