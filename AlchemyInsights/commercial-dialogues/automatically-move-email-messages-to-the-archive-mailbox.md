---
title: Déplacer automatiquement les messages électroniques vers la boîte aux lettres d’archivage
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059224"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Déplacer automatiquement les messages électroniques vers la boîte aux lettres d’archivage

Voici comment configurer une stratégie pour déplacer automatiquement l’ancien courrier électronique d’un utilisateur vers la boîte aux lettres d’archivage :

1. Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data  >  **governance**  >  **Archive** to verify an archive mailbox has been enabled for the user. Si ce n’est pas le cas, cliquez sur **Activer,** **puis Oui** dans la zone d’avertissement.
2. Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Choisissez l’icône + puis **choisissez automatiquement s’appliquer à la boîte aux lettres entière.**
4. Attribuez un nom à la balise de rétention, puis choisissez **Déplacer vers l’archive.** Pour la période de rétention, entrez l’heure que vous souhaitez, par exemple 90 jours. Cliquez sur **Save (Enregistrer)**.
5. Maintenant, créez une stratégie de rétention : choisissez des **stratégies de** rétention, choisissez l’icône pour ajouter une nouvelle stratégie.
6. Attribuez un nom à la stratégie de rétention, puis cliquez et faites défiler pour rechercher et ajouter la balise de rétention que vous vient de créer. Cliquez sur **Save (Enregistrer)**.
7. Enfin, appliquez la stratégie de rétention à la boîte aux lettres de l’utilisateur : toujours dans le centre d’administration Exchange, allez aux **boîtes** aux lettres des  >  **destinataires.** Choisissez tous les utilisateurs à qui vous souhaitez appliquer la stratégie, puis sélectionnez **Modifier** (icône de crayon).
8. Dans la boîte de dialogue, cliquez sur **fonctionnalités de boîte aux lettres.** Sous **Stratégie de rétention,** appliquez la stratégie que vous avez créée > **Enregistrer.**
9. Pour obtenir des instructions sur l’application de la stratégie à tous les utilisateurs, voir [Appliquer une stratégie de rétention aux boîtes aux lettres.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
