---
title: Corriger les règles de transport
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034752"
---
# <a name="fix-transport-rules"></a>Corriger les règles de transport

Une règle de flux de messagerie personnalisée a affecté ce message. Pour passer en revue la règle exacte, faites les choses suivantes :

1. Dans les résultats de la soumission, sous **Informations supplémentaires,** notez le **GUID** ou le nom **de la stratégie.**
2. Lancez Exchange Management Shell. Pour plus d'informations, voir [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Exécutez cette commande (à l’aide du GUID de votre soumission) :  **Get-TransportRule -identity « GUID » | fl * Description***
4. Consultez la description pour voir les conditions configurées qui ont affecté le message.

Pour plus d’informations, [voir Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
