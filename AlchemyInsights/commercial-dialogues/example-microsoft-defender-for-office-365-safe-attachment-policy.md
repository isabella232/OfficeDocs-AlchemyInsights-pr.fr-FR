---
title: Exemple de stratégie de pièces jointes Microsoft Defender Office 365 Coffre pièces jointes
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988293"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exemple de stratégie de pièces jointes Microsoft Defender Office 365 Coffre pièces jointes

Ces paramètres activent une stratégie appelée *Aucun* délai qui fournit les messages immédiatement, puis réattaque les pièces jointes après leur analyse :

- **Nom**: aucun délai
- **Description**: fournit les messages immédiatement et réattaque les pièces jointes après analyse.
- **Réponse**: sélectionnez **l’option Remise** dynamique. Pour plus d’informations, [voir Remise dynamique dans Coffre stratégies de pièces jointes.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Section** Rediriger les pièces jointes : sélectionnez l’option Activer la **redirection,** puis entrez l’adresse e-mail de votre administrateur général Microsoft 365, administrateur de sécurité ou analyste de sécurité qui étudiera les pièces jointes malveillantes.
- **Section Appliqué à** : **Sélectionnez le domaine du destinataire,** puis sélectionnez votre domaine. Sélectionnez **Ajouter,** puis **OK**. Une fois que vous avez terminé, sélectionnez **Enregistrer.**

Pour plus d’informations, [voir Coffre pièces jointes dans Microsoft Defender pour Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
