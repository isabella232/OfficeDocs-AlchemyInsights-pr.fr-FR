---
title: Une erreur de validation d'erreur de jeton d'accès s'est produite lors de l'embarquement d'Analyses du bureau
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813686"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erreur « Une erreur s'est produite lors de la validation du jeton d'accès » lors de l'intégration de Desktop Analytics

Cette erreur est normalement observée à l'expiration du jeton d'authentification. En règle générale, l'actualisation de la page actualisé le jeton. Toutefois, ce problème peut persister s'il existe des stratégies d'accès conditionnel appliquées au compte utilisé pour l'analyse du bureau à bord. Vous pouvez consulter les journaux de connexion Azure AD dans le portail Azure pour voir s'il existe des échecs de connexion pour le compte utilisé pour l'intégration d'Analyses du bureau.

Pour plus d'informations sur l'accès conditionnel, voir [Planifier votre déploiement d'accès conditionnel.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)