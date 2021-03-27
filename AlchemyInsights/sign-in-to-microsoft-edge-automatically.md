---
title: Se connectez automatiquement à Microsoft Edge
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398727"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Se connectez automatiquement à Microsoft Edge

Microsoft Edge utilise le compte par défaut du système d’exploitation pour se connecter automatiquement à un utilisateur en fonction de la configuration de son appareil. 

Les scénarios de chaque type de configuration d’appareil et de son processus de signature utilisateur dépendant sont décrits ci-dessous :

- **L’appareil est hybride/AAD-J**: cette option est disponible sur Windows 10, Windows de bas niveau et les versions serveur correspondantes. Les utilisateurs sont automatiquement signés avec leurs comptes Azure Active Directory (AD).
- **L’appareil est joint au** domaine : cette option est disponible sur Windows 10, Windows de bas niveau et les versions de serveur correspondantes. Par défaut, les utilisateurs ayant des comptes de domaine ne sont pas automatiquement signés ; pour activer la signature automatique pour eux, utilisez la **stratégie ConfigureOnPremisesAccountAutoSignIn.** Pour activer la connectez-vous automatique pour les utilisateurs ayant des comptes Azure AD, envisagez de rejoindre leurs appareils de façon hybride.
- Le compte par défaut du système **d’exploitation** est un compte Microsoft : cette option est disponible sur Windows 10 RS3 (version 1709, build 10.0.16299) et versions ultérieures. Il est peu probable que le scénario se produise sur les appareils d’entreprise. Toutefois, si le compte par défaut du système d’exploitation est un compte Microsoft, Microsoft Edge se connecte automatiquement à l’utilisateur avec le compte Microsoft.
 
 
