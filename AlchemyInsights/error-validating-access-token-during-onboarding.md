---
title: Une erreur s’est produite lors de la validation de l’erreur de jeton d’accès lors de l’intégration de l’analyse de bureau
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741172"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erreur « une erreur de validation du jeton d’accès » s’est produite lors de l’intégration de l’analyse de bureau

Cette erreur est normalement observée lorsque le jeton d’authentification arrive à expiration. En règle générale, l’actualisation de la page actualise le jeton. Toutefois, ce problème peut persister si des stratégies d’accès conditionnel sont appliquées au compte utilisé pour l’analyse de bureau intégrée. Vous pouvez consulter les journaux de connexion Azure AD dans le portail Azure pour voir s’il existe des échecs de connexion pour le compte utilisé pour l’intégration de l’analyse de bureau.

Pour plus d’informations sur l’accès conditionnel, consultez [la rubrique planifier votre déploiement d’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).