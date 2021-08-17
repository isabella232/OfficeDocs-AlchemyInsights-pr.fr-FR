---
title: Connectez-vous Microsoft Edge automatiquement
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050692"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Connectez-vous Microsoft Edge automatiquement

Microsoft Edge utilise le compte par défaut du système d’exploitation pour se connecter automatiquement à un utilisateur en fonction de la configuration de son appareil. 

Les scénarios de chaque type de configuration d’appareil et de son processus de signature utilisateur dépendant sont décrits ci-dessous :

- **L’appareil est hybride/AAD-J**: cette option est disponible sur les Windows 10, les Windows de bas niveau et les versions de serveur correspondantes. Les utilisateurs sont automatiquement signés avec Azure Active Directory comptes (AD).
- **L’appareil est joint au** domaine : cette option est disponible sur les Windows 10, les Windows de bas niveau et les versions de serveur correspondantes. Par défaut, les utilisateurs ayant des comptes de domaine ne sont pas automatiquement signés . pour activer la sign-in automatique pour eux, utilisez la **stratégie ConfigureOnPremisesAccountAutoSignIn.** Pour activer la connectez-vous automatique pour les utilisateurs ayant des comptes Azure AD, envisagez de rejoindre leurs appareils de façon hybride.
- Le compte par défaut du système **d’exploitation** est un compte Microsoft : cette option est disponible sur Windows 10 RS3 (version 1709, build 10.0.16299) et les versions ultérieures. Il est peu probable que le scénario se produise sur les appareils d’entreprise. Toutefois, si le compte par défaut du système d’exploitation est un compte Microsoft, Microsoft Edge se connecte automatiquement à l’utilisateur avec le compte Microsoft.
 
 
