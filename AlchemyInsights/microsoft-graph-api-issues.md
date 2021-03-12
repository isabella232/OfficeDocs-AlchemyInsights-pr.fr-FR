---
title: Problèmes de l’API Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716197"
---
# <a name="microsoft-graph-api-issues"></a>Problèmes de l’API Microsoft Graph

Cette rubrique peut également s’appliquer aux développeurs qui utilisent encore l’API Azure AD Graph. Toutefois, il **est vivement recommandé** d’utiliser Microsoft Graph pour tous vos scénarios de gestion des annuaires, des identités et des accès.

**Problèmes d’authentification ou d’autorisation**

- Si votre application ne parvient pas à acquérir des jetons pour appeler Microsoft Graph, sélectionnez Problème d’obtention d’une catégorie de jeton d’accès **(authentification)** Microsoft Graph pour obtenir une aide et un support plus **spécifiques** sur cette rubrique.
- Si votre application reçoit des erreurs d’autorisation **401 ou 403** lors de l’appel de Microsoft Graph, sélectionnez la catégorie d’API Microsoft Graph Obtention d’une erreur d’accès refusé **(autorisation)** pour obtenir une aide et un support plus spécifiques sur cette rubrique.

**Je veux utiliser Microsoft Graph, mais je ne sais pas par où commencer**

- [Présentation de Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Vue d’ensemble de la gestion des identités et des accès dans Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Commencer à créer des applications Microsoft Graph](https://docs.microsoft.com/graph/)
- **Explorateur Microsoft Graph** : tester les API Microsoft Graph dans votre client ou un client de démonstration

**Je veux utiliser Microsoft Graph, mais prend-il en charge les API d’annuaire v1.0 dont j’ai besoin ?**

Microsoft Graph est l’API recommandée pour la gestion des répertoires, des identités et des accès. Toutefois, il existe encore quelques lacunes entre ce qui est possible dans Azure AD Graph et Microsoft Graph. Lisez les articles suivants, qui mettent en évidence les différences les plus à jour pour vous aider dans votre choix :

- [Différences de type de ressource entre Azure AD Graph et Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Différences de propriétés entre Azure AD Graph et Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Différences de méthode entre Azure AD et Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**L’API que j’appelle ne fonctionne pas: où puis-je faire d’autres tests ?**

**Explorateur Microsoft Graph** : testez les API Microsoft Graph dans  votre client ou un client de démonstration et consultez également les exemples de requêtes dans l’Explorateur Microsoft Graph.

**Mon application est trop lente et est également limitée. Quelles améliorations puis-je apporter ?**

Selon votre scénario, plusieurs options sont à votre disposition pour rendre votre application plus performante et, dans certains cas, moins susceptible d’être limitée par le service (lorsque vous faites trop d’appels).

- [Meilleures pratiques de Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Traitement par lots de demandes](https://docs.microsoft.com/graph/json-batching)
- [Suivre les modifications par le biais d’une requête delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Être averti des modifications apportées par le biais de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Recommandations en cas de limitation](https://docs.microsoft.com/graph/throttling)

**Où puis-je trouver plus d’informations sur les erreurs et les problèmes connus ?**

- [Informations sur la réponse d’erreur Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problèmes connus avec Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Où puis-je vérifier l’état de la disponibilité et de la connectivité du service ?**

La disponibilité et la connectivité des services sous-jacents accessibles via Microsoft Graph peuvent avoir un impact sur la disponibilité et les performances globales de Microsoft Graph.

- Pour l’état du service Azure Active Directory, vérifiez l’état des services **Sécurité + Identité** répertoriés dans la page [d’état Azure.](https://azure.microsoft.com/status/)
- Pour les services Office qui contribuent à Microsoft Graph, vérifiez l’état des services répertoriés dans le tableau de bord d’état [du service Office.](https://portal.office.com/adminportal/home#/servicehealth)

Les erreurs d’autorisation de Microsoft Graph peuvent être le résultat de plusieurs problèmes différents, dont la plupart génèrent une erreur 401 ou 403. Par exemple, les problèmes suivants peuvent donner lieu à des erreurs d’autorisation :

- [Flux d’acquisition de jetons d’accès](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorrects
- Mauvaise configuration des [étendues d’autorisations](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Absence de [consentement](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Fin du support de la Bibliothèque d'authentification Active Directory (ADAL) et de l’API Azure AD Graph (AAD Graph)_* _

_*À compter du 30 juin 2020**, nous n’ajouterons plus de nouvelles fonctionnalités à ADAL et Azure AD Graph. Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.

**À compter du 30 juin 2022,** nous arrêterons la prise en charge d’ADAL et d’Azure AD Graph et ne fournirons plus de support technique ni de mises à jour de sécurité.

Les applications utilisant ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais n’auront pas de support technique ou de mises *à jour de sécurité.*

Les applications utilisant Azure AD Graph après cette période peuvent ne plus recevoir de réponses du point de terminaison Azure AD Graph.

**ADAL Migration**

Nous vous recommandons d’effectuer la mise à jour vers la [Bibliothèque d’authentification Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), qui contient les dernières fonctionnalités et mises à jour de sécurité.

Si vous utilisez des applications Microsoft, sachez que Microsoft est en train de migrer ses applications vers MSAL à l’échéance de fin du support, en veillant à ce qu’elles bénéficient des améliorations constantes en matière de sécurité et de fonctionnalités de MSAL.

1. [Lisez la FAQ sur la bibliothèque ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [En savoir plus sur la migration des applications selon la plateforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Si vous avez besoin d’aide pour savoir quelles applications utilisent ADAL, nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, de joindre des fournisseurs de logiciels indépendants ou des fournisseurs d’applications. L’équipe Support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre locataire (tenant).

**Migration des applications AAD Graph**

Pour les applications qui utilisent Azure AD Graph, suivez nos instructions pour migrer des applications [Azure AD Graph vers Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Notre liste de vérification de la migration fournit un point de mise en route](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Votre portail d’inscription d’applications Azure indique les applications qui utilisent AAD Graph. Nous vous recommandons d’examiner le code source de toutes vos applications et, le cas échéant, de faire appel à un éditeur de logiciels ou à un fournisseur d’applications indépendant. Le support Microsoft peut également vous fournir une liste de toutes les utilisations d’AAD Graph dans votre client.
3. Pour que votre application puisse accéder aux données dans Microsoft Graph, l’utilisateur ou l’administrateur doivent lui accorder les autorisations appropriées via un processus de consentement. La [référence des autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) répertorie les autorisations associées à chaque ensemble majeur d’API Microsoft Graph. Elle fournit également des instructions sur l’utilisation des autorisations.
