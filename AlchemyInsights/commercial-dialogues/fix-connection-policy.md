---
title: Corriger la stratégie de connexion
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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888404"
---
# <a name="fix-connection-policy"></a>Corriger la stratégie de connexion

L’e-mail a été marqué comme sécurisé et remis dans la boîte de réception de l’utilisateur, car l’adresse IP source a été marquée comme fiable dans la stratégie de filtrage des connexions par défaut. Pour passer en revue la stratégie, vous pouvez suivre les étapes suivantes :

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> , go to Email & **Collaboration** Policies \> **& Rules** Threat \> **policies** \> **Anti-spam** in the **Policies** section.

   Pour accéder directement à la page **Stratégies anti-courrier indésirable**, utilisez <https://security.microsoft.com/antispam>.

2. Dans la page **Stratégies anti-courrier** indésirable, sélectionnez la stratégie nommée Stratégie de filtrage des connexions **(par défaut)** en cliquant sur le nom de la stratégie.

3. Dans le volet d’informations qui s’affiche, cliquez sur **Modifier** la stratégie de filtrage des connexions dans la section **Filtrage des** connexions.

4. Consultez les entrées de la section Toujours autoriser les messages  de la section **Adresses IP** ou plage d’adresses suivantes, et voir si activer la liste sécurisée est sélectionnée.

   > [!NOTE]
   > Microsoft souscrit à des sources tierces d'expéditeurs dignes de confiance. Si la liste fiable est activée, ces expéditeurs fiables ne sont pas marqués par erreur comme courrier indésirable. Nous vous recommandons de sélectionner cette option, car elle permet de réduire le nombre de faux positifs (bon courrier classé comme courrier indésirable) que vous recevez.

Pour plus d’informations, consultez [Configuration du filtrage des connexions](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
