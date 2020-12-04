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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571826"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concepts d’authentification avancés applicables à Microsoft Edge

Voici les concepts d’authentification avancés qui s’appliquent à Microsoft Edge :

**Authentification proactive**

Lorsque vous activez la stratégie [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge essaie d’authentifier de manière proactive les utilisateurs connectés via les services Microsoft. À intervalles réguliers, il utilise un service en ligne pour rechercher un manifeste mis à jour qui contient la configuration régissant l’authentification proactive.

Avantages : l’authentification proactive permet l’authentification à des services clés, tels que la page Office New Tab. De plus, si Bing est utilisé comme moteur de recherche, l’authentification proactive améliore les performances de la barre d’adresses et génère des résultats de recherche personnalisés pour répondre aux besoins de votre entreprise.

**Windows Hello CredUI pour l’authentification NTLM**

Si l’authentification unique (SSO) n’est pas disponible lorsqu’un site Web tente de se connecter à l’utilisateur par le biais du mécanisme NTLM ou Negotiate, cette fonctionnalité permet à l’utilisateur de partager les informations d’identification du système d’exploitation avec le site Web et de satisfaire la stimulation d’authentification à l’aide de l’interface utilisateur Windows Hello CRED. Ce flux d’authentification s’affiche uniquement dans Windows 10 et uniquement pour les utilisateurs qui n’obtiennent pas d’authentification unique pendant une stimulation NTLM ou Negotiate.

**Utiliser des mots de passe enregistrés pour se connecter automatiquement**

Les utilisateurs qui enregistrent des mots de passe dans Microsoft Edge peuvent activer la connexion automatique aux sites Web où ils ont enregistré des informations d’identification. Les utilisateurs peuvent activer ou désactiver cette fonctionnalité dans edge://settings/passwords, et vous pouvez les configurer dans les stratégies du [Gestionnaire de mots de passe](https://go.microsoft.com/fwlink/?linkid=2134622) .
