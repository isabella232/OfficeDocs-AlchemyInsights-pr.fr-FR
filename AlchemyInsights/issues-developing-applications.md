---
title: Problèmes lors du développement d’applications
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950734"
---
# <a name="issues-developing-applications"></a>Problèmes lors du développement d’applications

Pour résoudre les problèmes les plus courants lors de la création d’applications Azure Active Directory (AD), veuillez consulter les articles suivants :

- [J’ai des problèmes de connexion à une ou plusieurs applications à l’aide du navigateur Chrome uniquement](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications). 
- [Je ne sais pas comment modifier les valeurs par défaut de la durée de vie des jetons pour mon application](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Je suis perplexe quant au fonctionnement du consentement concernant les applications](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Je ne sais pas comment accorder des autorisations à mon application](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Je ne comprends pas la différence entre les autorisations déléguées et les autorisations d’application](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Fin de la prise en charge de la Bibliothèque d’authentification Azure Active Directory (ADAL) et de l’API Azure AD Graph (AAD Graph)** _

- À compter du 30 juin 2020, nous n’ajouterons plus de nouvelles fonctionnalités à la Bibliothèque d’authentification Azure Active Directory (ADAL) et à l’API Azure AD Graph (AAD Graph). Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.

- À compter du 30 juin 2022, nous allons mettre fin à la prise en charge de la bibliothèque ADAL et d’AAD Graph ; nous ne fournirons plus de support technique, ni de mises à jour de sécurité. Par conséquent, les implications sont les suivantes :

    - Les applications qui utilisent ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais ne bénéficieront pas d’un quelconque support technique, ni de mises à jour de sécurité.

    - Les applications utilisant Azure AD Graph après cette période risquent de ne plus recevoir de réponses du point de terminaison AAD Graph.

_ *Migration de la bibliothèque ADAL**

Si vous utilisez des applications Microsoft, nous vous recommandons d’effectuer la mise à jour vers la bibliothèque d’authentification Microsoft (MSAL), qui contient les dernières fonctionnalités et mises à jour de sécurité. Nous émettons cette recommandation dans le contexte suivant : Microsoft a lancé le processus de migration de ses applications vers la bibliothèque MSAL avant la fin du support technique. 

La migration, par Microsoft, de ses applications vers la bibliothèque MSAL garantit que les applications bénéficient des améliorations constantes apportées par cette bibliothèque en matière de sécurité et de fonctionnalités.

1. [Lisez la FAQ sur la bibliothèque ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [En savoir plus sur la migration des applications selon la plateforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Si vous avez besoin d’aide pour comprendre quelles sont vos applications qui utilisent ADAL, nous vous recommandons d’évaluer le code source de toutes vos applications et, le cas échéant, de faire appel à des éditeurs de logiciels indépendants ou à des fournisseurs d’applications. Le support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre client.

**Migration des applications AAD Graph**

Veuillez suivre nos recommandations pour migrer les applications AAD Graph vers Microsoft Graph :

1. [Notre liste de contrôle de la migration fournit un point de mise en route](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Votre portail d’inscription d’applications Azure indique les applications qui utilisent AAD Graph. Nous vous recommandons d’évaluer le code source de toutes vos applications et, le cas échéant, de faire appel à des éditeurs de logiciels indépendants ou à des fournisseurs d’applications. Le support Microsoft peut également vous fournir des informations sur l’utilisation d’AAD Graph dans votre client.







