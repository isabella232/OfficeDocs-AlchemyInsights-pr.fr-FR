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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353504"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Rappeler ou remplacer un message électronique dans Microsoft 365

- Vous pouvez **uniquement rappeler les messages qui sont envoyés à des personnes de votre organisation**. Par exemple, si le message a été envoyé à une adresse Gmail, vous ne pouvez pas le rappeler.
- Vous **ne pouvez rappeler que les messages envoyés à partir d’Outlook pour le PC**. Si un utilisateur envoie un message à l’aide d’Outlook pour Mac ou d’Outlook sur le Web, vous ne pouvez pas le rappeler.
- En tant qu’administrateur client, vous pouvez **rappeler des messages au nom des utilisateurs à l’aide de PowerShell** (pour plus d’informations, consultez la rubrique : [Rechercher et supprimer des messages électroniques](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Vous ne pouvez pas rappeler les messages à partir du centre d’administration. Faites défiler vers le bas jusqu’à « rechercher et supprimer des messages électroniques dans votre organisation » pour plus d’informations.

**Rappeler ou remplacer un message électronique que vous avez envoyé**

1. Dans le volet des dossiers situé à gauche de la fenêtre Outlook, sélectionnez le dossier éléments envoyés.
2. Ouvrez le message que vous souhaitez rappeler. Vous devez double-cliquer pour ouvrir le message. La sélection du message de sorte qu’il s’affiche dans le volet de lecture ne vous permet pas de rappeler le message.
3. Dans l’onglet message, sélectionnez **actions**  >  **rappeler ce message**.
4. Choisissez **Supprimer les copies non lues de ce message** ou **Supprimer les copies non lues et les remplacer par un nouveau message**, puis cliquez sur **OK**.
5. Si vous envoyez un message de remplacement, composez le message, puis sélectionnez **Envoyer**.
6. La réussite ou l’échec d’un rappel de message dépend des paramètres des destinataires dans Outlook.

Pour plus d’informations, notamment sur la vérification du rappel, reportez-vous à la rubrique [rappeler ou remplacer un message électronique que vous avez envoyé](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Pour rechercher et supprimer des messages électroniques dans votre organisation_**, il est plus facile de le faire si vous êtes un administrateur général. Si vous n’êtes pas un administrateur général, votre compte doit être ajouté au groupe de rôles gestionnaire eDiscovery ou au rôle de gestion de la recherche de conformité. Pour supprimer des messages, vous devez rejoindre le groupe de rôles gestion de l’organisation ou le rôle de gestion de la recherche et de la purge. Les autorisations d’accès à ces rôles sont affectées dans le [Centre de sécurité & conformité](https://protection.office.com/).

1. [Créer une recherche de contenu](https://docs.microsoft.com/microsoft-365/compliance/content-search) pour rechercher le message à supprimer.
2. [Se connecter à l’interface PowerShell du Centre de sécurité et conformité](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Si vous utilisez l’authentification multifacteur (MFA), consultez [la rubrique Connect to Microsoft 365 Security & Compliance Center PowerShell using Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
