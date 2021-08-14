---
title: Interrogation de l’API microsoft Graph
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923237"
---
# <a name="querying-the-microsoft-graph-api"></a>Interrogation de l’API microsoft Graph

Cette rubrique peut également s’appliquer aux développeurs qui utilisent encore Azure AD Graph API. Toutefois, il **est vivement recommandé** d’utiliser Microsoft Graph pour tous vos scénarios de gestion des annuaires, des identités et des accès.

**Problèmes d’authentification ou d’autorisation**

- Si votre  application ne parvient pas à acquérir des jetons pour appeler Microsoft Graph, sélectionnez Problème d’obtention d’une catégorie de jeton d’accès **(authentification)** Microsoft Graph pour obtenir une aide et un support plus spécifiques sur cette rubrique.
- Si votre application reçoit des erreurs d’autorisation **401 ou 403** lors de l’appel de Microsoft Graph, sélectionnez la catégorie d’API Microsoft Graph Obtention d’une erreur d’accès refusé **(autorisation)** pour obtenir une aide et un support plus spécifiques sur cette rubrique.

**Je veux utiliser Microsoft Graph, mais je ne sais pas par où commencer**

Pour en savoir plus sur Microsoft Graph, voir :

- [Présentation de Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Vue d’ensemble de la gestion des identités et des accès dans Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Mise en place de la création d Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** : tester les API microsoft Graph client ou de démonstration

**Je souhaite utiliser Microsoft Graph, mais prend-il en charge les API d’annuaire v1.0 dont j’ai besoin ?**

Microsoft Graph l’API recommandée pour la gestion des répertoires, des identités et des accès. Toutefois, il existe encore quelques lacunes entre ce qui est possible dans Azure AD Graph et Microsoft Graph. Lisez les articles suivants, qui mettent en évidence les différences les plus à jour pour vous aider dans votre choix :

- [Différences de type de ressource entre Azure AD Graph et Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Différences de propriétés entre Azure AD Graph et Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Différences de méthodes entre Azure AD et Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Lorsque j’interroge *l’objet utilisateur,* la plupart de ses propriétés sont manquantes**

`GET https://graph.microsoft.com/v1.0/users`renvoie uniquement 11 propriétés, car Microsoft Graph sélectionne automatiquement un ensemble par défaut *de* propriétés utilisateur à renvoyer. Si vous avez besoin *d’autres* propriétés utilisateur, utilisez $select pour sélectionner les propriétés dont votre application a besoin. Essayez-le **d’abord dans l Graph’explorateur** Microsoft.

**Certaines valeurs de propriété utilisateur *sont null* même si je sais qu’elles sont définies**

L’explication la plus probable est que l’application a reçu l’autorisation *User.ReadBasic.All.* Cela permet à l’application de lire un ensemble limité de propriétés utilisateur, renvoyant toutes les autres propriétés comme null, même si elles ont été définies précédemment. Essayez plutôt d’accorder *l’autorisation User.Read.All* à l’application.

Pour plus d’informations, [voir Microsoft Graph’autorisations utilisateur.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**J’ai des difficultés à utiliser les paramètres de requête OData pour filtrer des données dans mes demandes**

Bien que Microsoft Graph prend en charge un large éventail de paramètres de requête OData, la plupart de ces paramètres ne sont pas entièrement pris en charge par les services d’annuaire (ressources qui héritent de *directoryObject*) dans Microsoft Graph. Les mêmes limitations qui étaient présentes dans Azure AD sont Graph la plupart du temps dans Microsoft Graph :

1. **Non pris en** charge : $count, $search et $filter sur des valeurs *null* *ou non null*
2. **Non pris en** charge : $filter sur certaines propriétés (voir les rubriques de ressources sur lesquelles les propriétés sont filtrables)
3. **Non pris en** charge : pagination, filtrage et tri en même temps
4. **Non pris en** charge : filtrage sur une relation. Par exemple, recherchez tous les membres du groupe d’ingénierie qui se trouvent au Royaume-Uni.
5. **Prise en charge** partielle : $orderby sur *l’utilisateur* (displayName et userPrincipalName uniquement) et le *groupe*
6. Prise en charge partielle : $filter (prend en charge uniquement *eq* *,* *startswith*, or , and , *and* limited *any*) support, $expand (le développement des relations d’un seul objet renvoie toutes les relations, mais le développement d’une collection de relations d’objets est limité)

Pour plus d’informations, voir [Personnaliser les réponses avec les paramètres de requête.](https://docs.microsoft.com/graph/query-parameters)

**L’API que j’appelle ne fonctionne pas: où puis-je faire d’autres tests ?**

**Microsoft Graph Explorer** : testez les API Microsoft Graph dans votre client ou  un client de démonstration et consultez également les exemples de requêtes dans l’Explorateur microsoft Graph.

**Lorsque j’interroge des données, j’ai l’impression d’obtenir un jeu de données incomplet**

Si vous interrogez une collection (comme les utilisateurs), Microsoft Graph utilise des limites de page côté serveur afin que les résultats soient toujours renvoyés avec une taille de page par défaut. Votre application doit toujours s’attendre à passer en page les collections renvoyées par le service.

Pour plus d’informations, voir :

- [Meilleures pratiques Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Pagination des données Microsoft Graph dans votre application](https://docs.microsoft.com/graph/paging)

**Mon application est trop lente et est également limitée. Quelles améliorations puis-je apporter ?**

Selon votre scénario, différentes options sont à votre disposition pour rendre votre application plus performante et, dans certains cas, moins susceptible d’être limitée par le service (lorsque vous faites trop d’appels).

Pour plus d’informations, voir :

- [Meilleures pratiques Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Demandes de traitement par lots](https://docs.microsoft.com/graph/json-batching)
- [Suivre les modifications par le biais d’une requête delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Être averti des modifications par le biais de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Recommandations en cas de limitation](https://docs.microsoft.com/graph/throttling)

**Où puis-je trouver plus d’informations sur les erreurs et les problèmes connus ?**

- [Informations de Graph d’erreur Microsoft](https://docs.microsoft.com/graph/errors)
- [Problèmes connus avec Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Où puis-je vérifier l’état de la disponibilité et de la connectivité du service ?**

La disponibilité et la connectivité des services sous-jacents accessibles via Microsoft Graph peuvent avoir un impact sur la disponibilité et les performances globales de Microsoft Graph.

- Pour Azure Active Directory l’état du service, vérifiez l’état des services **Sécurité + Identité** répertoriés dans la page [d’état Azure.](https://azure.microsoft.com/status/)
- Pour Office services qui contribuent à Microsoft Graph, vérifiez l’état des services répertoriés dans le tableau de bord [Office’état du service.](https://portal.office.com/adminportal/home#/servicehealth)
