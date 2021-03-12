---
title: Exemple de stratégie de pièces jointes sécurisées Microsoft Defender pour Office 365
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
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736748"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exemple de stratégie de pièces jointes sécurisées Microsoft Defender pour Office 365

Ces paramètres activent une stratégie appelée *Aucun* délai qui fournit les messages immédiatement, puis réattaque les pièces jointes après leur analyse :

- **Nom**: aucun délai
- **Description**: fournit les messages immédiatement et réattaque les pièces jointes après analyse.
- **Réponse**: sélectionnez **l’option Remise** dynamique. Pour plus d’informations, [voir Remise dynamique dans les stratégies de pièces jointes sécurisées.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Section** Rediriger les pièces jointes : sélectionnez l’option Activer la **redirection,** puis entrez l’adresse e-mail de votre administrateur général Microsoft 365, administrateur de sécurité ou analyste de sécurité qui étudiera les pièces jointes malveillantes.
- **Section Appliqué à** : **Sélectionnez le domaine du destinataire,** puis sélectionnez votre domaine. Sélectionnez **Ajouter,** puis **OK.** Une fois que vous avez terminé, sélectionnez **Enregistrer.**

Pour plus d’informations, [voir Pièces jointes sécurisées dans Microsoft Defender pour Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
