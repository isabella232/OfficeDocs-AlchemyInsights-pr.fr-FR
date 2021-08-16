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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988100"
---
# <a name="fix-connection-policy"></a>Corriger la stratégie de connexion

L’e-mail a été marqué comme sécurisé et remis dans la boîte de réception de l’utilisateur, car l’adresse IP d’envoi a été marquée comme étant sûre dans la stratégie de filtrage des connexions. Pour passer en revue la stratégie, faites les choses suivantes :

1. Go to the [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)and then go to Threat **management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Sous **l’onglet** Personnalisé, sélectionnez la stratégie de filtrage **des** connexions, puis **sélectionnez Modifier la stratégie.**
3. Examinez la **liste d’adresses IP** autoriser. Voir si **Coffre liste est** activée.

    > [!NOTE]
    > Microsoft souscrit à des sources tierces d'expéditeurs dignes de confiance. Si **Coffre liste** est activée, ces expéditeurs fiables ne sont pas marqués par erreur comme courrier indésirable. Je recommande de sélectionner cette option, car elle permet de réduire le nombre de faux positifs (bon courrier classé comme courrier indésirable) que vous recevez.
