---
title: Stratégies Catchall
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "3207"
ms.openlocfilehash: e5d08462e8662fa1651ad81235d0efd5fc4bac58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721292"
---
# <a name="teams-policies"></a>Stratégies teams

Les paramètres de Microsoft teams sont contrôlés par des stratégies. Pour effectuer une modification, vous devez configurer la stratégie appropriée, puis l’appliquer aux utilisateurs. Le moyen le plus rapide d’effectuer cette opération pour tous vos utilisateurs consiste à modifier la stratégie par défaut nommée global. 

**Note** Les modifications apportées aux stratégies prennent ***effet au moins 4 à 48 heures***. Si vous créez une stratégie personnalisée, vous devez attendre au moins 4 heures avant de pouvoir y effectuer des modifications supplémentaires. Vous pouvez ensuite appliquer cette stratégie aux utilisateurs. Cela signifie que les stratégies personnalisées peuvent prendre jusqu’à 48 heures. Les stratégies globales sont définies par défaut pour tous les utilisateurs et les modifications apportées à la stratégie globale peuvent prendre jusqu’à 24 heures. Si vous avez créé une stratégie personnalisée, l’avez appliquée aux utilisateurs, et qu’elle n’a toujours pas pris effet après 48 heures, ou si vous avez modifié la stratégie globale et que vous avez attendu au moins 24 heures, veuillez ouvrir un cas de support.

Les stratégies de teams sont réparties dans les domaines suivants :

- Les [stratégies teams](https://docs.microsoft.com/MicrosoftTeams/teams-policies) contrôlent la découverte des utilisateurs de teams privées lors de la recherche et de la création de canaux privés.  
- Les [stratégies de réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) contrôlent ce que les utilisateurs peuvent faire avec les réunions Teams, y compris le contrôle de la salle d’attente. Pour obtenir de l’aide sur les problèmes liés à la salle d’attente, comme la configuration de teams pour admettre tout le monde, voir [paramètres de la salle d’attente et niveaux de participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby)
- Les [stratégies de messagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) contrôlent ce que les utilisateurs peuvent faire de la conversation et des messages, notamment activer ou désactiver le mode conversation, supprimer des conversations, demander des confirmations de lecture, utiliser des images giphy et des autocollants, et bien plus encore.
- Les [stratégies de configuration d’application](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) contrôlent les applications disponibles pour les utilisateurs, notamment les applications personnalisées et tierces, ainsi que l’ordre dans lequel elles apparaissent.  
- Les [stratégies de rétention](https://docs.microsoft.com/microsoftteams/retention-policies) des données pour teams se trouvent dans le centre de sécurité et de conformité Microsoft 365.
- Les stratégies de carnet d’adresses teams sont définies par le biais de la recherche dans l' [Annuaire](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).