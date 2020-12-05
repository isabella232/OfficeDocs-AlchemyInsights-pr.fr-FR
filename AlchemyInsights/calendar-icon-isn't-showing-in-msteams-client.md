---
title: L’icône du calendrier n’est pas visible dans le client Microsoft teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576521"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>L’icône du calendrier n’est pas visible dans le client Microsoft teams

L’onglet **calendrier** dans teams nécessite l’accès à une boîte aux lettres Exchange via les services Web Exchange. La boîte aux lettres Exchange peut être en ligne ou en local. Pour les utilisateurs en ligne qui ne voient pas l’onglet **calendrier** , vérifiez qu’ils [disposent d’une licence pour une boîte aux lettres Exchange Online et que la boîte aux lettres est activée](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Si vos utilisateurs sont hébergés en local, vous devez vous assurer que votre configuration hybride est intègre. Utilisez l’ [Assistant configuration hybride](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pour résoudre les problèmes. Notez que [Teams nécessite Exchange 2016 CU3 ou une version ultérieure](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Pour plus d’informations et pour connaître les étapes de dépannage, consultez la rubrique [Troubleshoot Microsoft teams and Exchange Server interaction Problems](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
