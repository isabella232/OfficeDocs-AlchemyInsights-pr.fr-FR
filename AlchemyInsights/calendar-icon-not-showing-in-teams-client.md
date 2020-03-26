---
title: L’icône de calendrier n’apparaît pas dans le client Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931979"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>L’icône de calendrier n’apparaît pas dans le client Teams

L’onglet Calendrier dans Teams nécessite l’accès à une boîte aux lettres Exchange par l’entremise des Services Web Exchange. La boîte aux lettres Exchange peut être en ligne ou en local. Pour les utilisateurs en ligne ne disposant pas de l’onglet Calendrier, assurez-vous qu’ils [sont titulaires d’une licence pour une boîte aux lettres Exchange Online et que la boîte aux lettres est activée](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Si l’utilisateur dispose d’une boîte aux lettres valide dans Exchange Online, mais ne peut pas consulter l’onglet Calendrier, il est possible que vous rencontriez un problème de réseau. Utilisez l’ [Analyseur de connectivité à distance Microsoft](https://testconnectivity.microsoft.com/) et exécutez les **tests de connectivité des services Web Microsoft Exchange** pour l’utilisateur concerné.

Activez la case à cocher [Applications Teams - stratégies de configuration pour l’application](https://admin.teams.microsoft.com/policies/app-setup) Pour vérifier que l’application calendrier n’a pas été supprimée de la stratégie appliquée à l’utilisateur (il s’agit probablement de**Global (par défaut à l’échelle de l’organisation)**.

Si vos utilisateurs sont hébergés en local, vous devez vérifier que votre configuration hybride est saine. Utilisez l’ [Assistant configuration hybride](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pour résoudre les problèmes.

Notez que [Teams nécessite Exchange 2016 CU3 ou une version ultérieure](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
