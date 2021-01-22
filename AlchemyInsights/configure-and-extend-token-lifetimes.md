---
title: Configurer et étendre la durée de vie des jetons
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911995"
---
# <a name="configure-and-extend-token-lifetimes"></a>Configurer et étendre la durée de vie des jetons

Vous pouvez spécifier la durée de vie d’un jeton d’accès, SAML, ou d’identification émis par la plateforme d’identité Microsoft. Vous pouvez définir les durées de vie des jetons pour toutes les applications de votre organisation, pour une application mutualisée (multi-organisation) ou pour un principal de service spécifique dans votre organisation. Pour plus d’informations, lisez [Durée de vie des jetons configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Pour consulter des exemples, [Exemples de la configuration de durées de vie des jetons](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Pour découvrir comment configurer la durée de vie et la compatibilité d’un jeton dans Azure Active Directory B2C (Azure AD B2C), consultez[Configurer des jetons dans Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

L’article [Configurer le comportement des sessions dans Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) décrit les méthodes d’authentification unique (SSO) utilisées dans Azure AD B2C et vous aide à choisir la méthode d’authentification unique la plus appropriée lors de la configuration de votre stratégie.

**Durée de vie des jetons, durée de validité des jetons**

La durée de vie des jetons est 1 heure et la durée de vie des sessions est 24 heures. Cela signifie que si aucune demande n’est faite au cours des 24 heures, vous devrez vous connecter à nouveau avant de demander un nouveau jeton.

> [!NOTE]
> Après le 30 mai 2020, aucun nouveau client ne pourra utiliser une stratégie de durée de vie des jetons configurable pour configurer des sessions et actualiser des jetons. Le dépréciation se produira plusieurs mois après, ce qui signifie que nous dépasserons les sessions existantes pour actualiser les stratégies des jetons. Vous pouvez toujours configurer les durées de vie des jetons d’accès après la dépréciation.






