---
title: L’icône Calendrier ne s’affiche pas dans Microsoft Teams client
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120002"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>L’icône Calendrier ne s’affiche pas dans Microsoft Teams client

**L’onglet** Calendrier dans Teams nécessite l’accès à une boîte Exchange aux lettres via Exchange Web Services. La Exchange boîte aux lettres peut être en ligne ou en local. Pour les utilisateurs en  ligne qui ne voient pas l’onglet Calendrier, assurez-vous qu’ils ont une licence pour une boîte aux lettres Exchange Online et que la boîte aux lettres [est activée.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Si vos utilisateurs sont homed On-Premises, vous devez vérifier que votre configuration hybride est saine. Utilisez l’ [Assistant configuration hybride](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pour résoudre les problèmes. Notez que [Teams nécessite Exchange 2016 CU3 ou une version ultérieure](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Pour plus d’informations et pour la résolution des problèmes, voir Résoudre Microsoft Teams [problèmes Exchange Server’interaction.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
