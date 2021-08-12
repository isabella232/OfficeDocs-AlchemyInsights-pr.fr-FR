---
title: Une erreur de validation du jeton d’accès s’est produite lors de l’embarquement d’Analyses du bureau
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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946613"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erreur « Une erreur s’est produite lors de la validation du jeton d’accès » lors de l’intégration de Desktop Analytics

Cette erreur est normalement observée à l’expiration du jeton d’authentification. En règle générale, l’actualisation de la page actualise le jeton. Toutefois, ce problème peut persister s’il existe des stratégies d’accès conditionnel appliquées au compte utilisé pour l’analyse du bureau à bord. Vous pouvez consulter les journaux de connexion Azure AD dans le portail Azure pour voir s’il existe des échecs de connexion pour le compte utilisé pour l’intégration d’Analyses du bureau.

Pour plus d’informations sur l’accès conditionnel, voir [Planifier votre déploiement d’accès conditionnel.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)