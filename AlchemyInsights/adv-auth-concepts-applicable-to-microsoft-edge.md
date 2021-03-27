---
title: Concepts d’authentification avancés applicables à Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398558"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concepts d’authentification avancés applicables à Microsoft Edge

Voici les concepts d’authentification avancés applicables à Microsoft Edge :

**Authentification proactive**

Lorsque vous activez la stratégie [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge tente d’authentifier de manière proactive les utilisateurs inscrits via les services Microsoft. À intervalles réguliers, il utilise un service en ligne pour vérifier un manifeste mis à jour qui contient la configuration régissant l’authentification proactive.

Avantages : l’authentification proactive permet l’authentification à des services clés, tels que la page Nouvel onglet Office. En outre, si Bing est utilisé comme moteur de recherche, l’authentification proactive améliore les performances de la barre d’adresses et permet de générer des résultats de recherche personnalisés en fonction des besoins de votre entreprise.

**Windows Hello CredUI pour l’authentification NTLM**

Si l’authentification unique (SSO) n’est pas disponible lorsqu’un site web tente de se connecter à l’utilisateur via le mécanisme NTLM ou Negotiate, cette fonctionnalité permet à l’utilisateur de partager les informations d’identification du système d’exploitation avec le site web et de répondre au défi d’authentification à l’aide de Windows Hello Cred UI. Ce flux d' sign-on s’affiche uniquement dans Windows 10 et uniquement pour les utilisateurs qui n’obtiennent pas d' SSO pendant une demande NTLM ou Negotiate.

**Utiliser des mots de passe enregistrés pour se connecter automatiquement**

Les utilisateurs qui enregistrent des mots de passe dans Microsoft Edge peuvent activer la connexion automatique aux sites web où ils ont enregistré des informations d’identification. Les utilisateurs peuvent activer ou désactiver cette fonctionnalité dans edge://settings/passwords, et vous pouvez la configurer dans les stratégies du [gestionnaire de mots de](https://go.microsoft.com/fwlink/?linkid=2134622) passe.
