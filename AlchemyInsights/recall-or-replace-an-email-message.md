---
title: Rappeler ou remplacer un message électronique
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024384"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Rappeler ou remplacer un message électronique dans Microsoft 365

- Vous pouvez **uniquement rappeler les messages envoyés à des personnes de votre organisation.** Par exemple, si le message a été envoyé à une adresse Gmail, vous ne pouvez pas le rappeler.
- Vous ne pouvez **rappeler que les messages envoyés Outlook pour le PC.** Si un utilisateur envoie un message à l’Outlook pour Mac ou Outlook sur le web, vous ne pouvez pas le rappeler.
- En tant qu’administrateur client, vous pouvez rappeler des messages au nom des utilisateurs à l’aide de **PowerShell** (pour plus d’informations, voir : Rechercher et supprimer [des messages électroniques).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Vous ne pouvez pas rappeler les messages du Centre d’administration. Faites défiler vers le bas jusqu’à « Rechercher et supprimer des messages électroniques dans votre organisation » pour plus d’informations.

**Rappeler ou remplacer un message électronique que vous avez envoyé**

1. Dans le volet de dossiers à gauche de la fenêtre Outlook, choisissez le dossier Éléments envoyés.
2. Ouvrez le message que vous souhaitez rappeler. Vous devez double-cliquer pour ouvrir le message. La sélection du message afin qu’il apparaisse dans le volet de lecture ne vous permettra pas de rappeler le message.
3. Sous l’onglet Message, **sélectionnez Actions**  >  **rappeler ce message.**
4. Choose **Delete unread copies of this message** or Delete **unread copies and replace with a new message,** then select **OK**.
5. Si vous envoyez un message de remplacement, composez-le, puis sélectionnez **Envoyer.**
6. La réussite ou l’échec d’un rappel de message dépend des paramètres des destinataires Outlook.

Pour plus d’informations, notamment sur la façon de vérifier le rappel, voir Rappeler ou [remplacer un message électronique que vous avez envoyé.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Pour rechercher et supprimer des messages électroniques*** dans votre organisation, il est plus facile si vous êtes un administrateur global. Si vous n’êtes pas un administrateur général, votre compte doit être ajouté au groupe de rôles Gestionnaire eDiscovery ou au rôle de gestion recherche de conformité. Pour supprimer des messages, vous devez rejoindre le groupe de rôles Gestion de l’organisation ou le rôle de gestion recherche et purge. Les autorisations sur ces rôles sont attribuées dans le [Centre de sécurité & conformité.](https://protection.office.com/)

1. [Créez une recherche de](https://docs.microsoft.com/microsoft-365/compliance/content-search) contenu pour rechercher le message à supprimer.
2. [Se connecter à l’interface PowerShell du Centre de sécurité et conformité](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Si vous utilisez l’authentification multifacteur( MFA), consultez l’Connecter pour Microsoft 365 Security & Compliance Center PowerShell à l’aide de l’authentification [multifacteur.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
