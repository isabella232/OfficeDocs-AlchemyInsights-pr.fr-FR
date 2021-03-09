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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568496"
---
# <a name="fix-connection-policy"></a>Corriger la stratégie de connexion

L’e-mail a été marqué comme sécurisé et remis dans la boîte de réception de l’utilisateur, car l’adresse IP d’envoi a été marquée comme étant sûre dans la stratégie de filtrage des connexions. Pour passer en revue la stratégie, faites les choses suivantes :

1. Go to the [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)and then go to **Threat management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Sous **l’onglet** Personnalisé, sélectionnez la stratégie **de filtrage des** connexions, puis sélectionnez Modifier la **stratégie.**
3. Examinez la **liste d’adresses IP** autoriser. Voir si **la liste sécurisée** est activée.

    > [!NOTE]
    > Microsoft souscrit à des sources tierces d'expéditeurs dignes de confiance. Si **la liste fiable** est activée, ces expéditeurs fiables ne sont pas marqués par erreur comme courrier indésirable. Je recommande de sélectionner cette option, car elle permet de réduire le nombre de faux positifs (bon courrier classé comme courrier indésirable) que vous recevez.
