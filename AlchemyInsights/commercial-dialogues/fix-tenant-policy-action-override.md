---
title: Corriger la stratégie de client (remplacement d’action)
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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034932"
---
# <a name="fix-tenant-policy-action-override"></a>Corriger la stratégie de client (remplacement d’action)

Une stratégie anti-courrier indésirable dans votre client a affecté ce message. Pour passer en revue la stratégie, faites les choses suivantes :

1. Go to the [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)and then go to Threat **management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Vérifiez si la **source de** stratégie indique les éléments suivants :  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Si c’est le cas, sous **l’onglet** Personnalisé, vérifiez les paramètres de la stratégie qui a affecté le message. Il est possible que les **paramètres Standard appliqués** à tous les clients Exchange Online Protection le message.

Pour plus d’informations sur la configuration des stratégies de filtrage du courrier indésirable, voir [Configurer vos stratégies de filtrage du courrier indésirable.](https://go.microsoft.com/fwlink/?linkid=2101431)
