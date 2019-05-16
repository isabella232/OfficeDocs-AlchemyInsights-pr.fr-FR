---
title: Rappeler ou remplacer un message électronique
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096494"
---
# <a name="recall-or-replace-an-email-message"></a>Rappeler ou remplacer un message électronique

- Vous pouvez **uniquement rappeler les messages qui sont envoyés à des personnes de votre organisation**. Si le message a été envoyé à une adresse Gmail, par exemple, vous ne pouvez pas le rappeler.
- Vous pouvez **uniquement rappeler les messages envoyés à partir d’Outlook 2016 pour le PC**. Si un utilisateur envoie un message à l’aide d’Outlook pour Mac ou d’Outlook sur le Web, vous ne pouvez pas le rappeler.
- Si vous êtes administrateur, vous pouvez **rappeler des messages au nom des utilisateurs à l’aide de PowerShell**. Vous ne pouvez pas rappeler les messages à partir du centre d’administration. Faites défiler vers le bas jusqu’à «rechercher et supprimer des messages électroniques dans votre organisation» pour plus d’informations.

***Rappeler ou remplacer un message électronique que vous avez envoyé***
1. Dans le volet des dossiers situé à gauche de la fenêtre Outlook, sélectionnez le dossier éléments envoyés.
2. Ouvrez le message que vous souhaitez rappeler. Vous devez double-cliquer pour ouvrir le message. La sélection du message de sorte qu’il s’affiche dans le volet de lecture ne vous permet pas de rappeler le message.
3. Dans l’onglet message, sélectionnez **actions** > **rappeler ce message**.
4. Choisissez **Supprimer les copies non lues de ce message** ou **Supprimer les copies non lues et les remplacer par un nouveau message**, puis cliquez sur **OK**.
5. Si vous envoyez un message de remplacement, composez le message, puis sélectionnez **Envoyer**.
6. La réussite ou l’échec d’un rappel de message dépend des paramètres des destinataires dans Outlook. 

Pour plus d’informations, notamment sur la vérification du rappel, reportez-vous à la rubrique [rappeler ou remplacer un message électronique que vous avez envoyé](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Rechercher et supprimer des messages électroniques dans votre organisation*** Pour rechercher et supprimer des messages électroniques dans votre organisation, il est plus facile de le faire si vous êtes un administrateur général. Si vous n’êtes pas un administrateur général, votre compte doit être ajouté au groupe de rôles gestionnaire eDiscovery ou au rôle de gestion de la recherche de conformité. Pour supprimer des messages, vous devez rejoindre le groupe de rôles gestion de l’organisation ou le rôle de gestion de la recherche et de la purge. Les autorisations sur ces rôles sont affectées dans le [Centre de sécurité & Compliance Center](https://protection.office.com/).

1. [Créer une recherche de contenu](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) pour rechercher le message à supprimer.
2. [Connectez-vous au centre de sécurité _AMP_ Compliance Center PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Si vous utilisez MFA, voir [Connect to Office 365 Security _AMP_ Compliance Center PowerShell using Multi-Factor Authentication](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 