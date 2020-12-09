---
title: Se connecter automatiquement à Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599467"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Se connecter automatiquement à Microsoft Edge

Microsoft Edge utilise le compte par défaut du système d’exploitation pour se connecter automatiquement à un utilisateur en fonction de la configuration de l’appareil de l’utilisateur. 

Les scénarios de chaque type de configuration d’appareil et de processus de connexion de l’utilisateur dépendant sont décrits ci-dessous :

1. **L’appareil est hybride/AAD-J**: cette option est disponible sur Windows 10, des fenêtres de bas niveau et des versions de serveur correspondantes. Les utilisateurs sont automatiquement connectés avec leurs comptes Azure Active Directory (AD).
2. **L’appareil est joint à un domaine**: cette option est disponible dans Windows 10, les fenêtres de bas niveau et les versions de serveur correspondantes. Par défaut, les utilisateurs disposant de comptes de domaine ne sont pas connectés automatiquement ; pour activer la connexion automatique, utilisez la stratégie **ConfigureOnPremisesAccountAutoSignIn** . Pour activer la connexion automatique pour les utilisateurs disposant de comptes Azure AD, envisagez la jonction hybride de leurs appareils.
3. **Le compte par défaut du se est un compte Microsoft**: cette option est disponible sur Windows 10 RS3 (version 1709, Build 10.0.16299) et les versions ultérieures. Il est peu probable que le scénario se produise sur les appareils de l’entreprise. Toutefois, si le compte par défaut du système d’exploitation est un compte Microsoft, Microsoft Edge se connectera automatiquement à l’utilisateur avec le compte Microsoft.
 
 
