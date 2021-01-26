---
title: Problèmes de développement d’applications avec des API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951899"
---
# <a name="issues-developing-applications-with-apis"></a>Problèmes de développement d’applications avec des API

Pour commencer à utiliser l’API Azure Active Directory Graph, consultez le guide de démarrage rapide de [l’API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ou consultez la documentation de référence interactive de l’API Azure [AD Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Fin de la prise en charge d’Azure Active Directory Authentication Library (ADAL) et de l’API Azure AD Graph (AAD Graph)**

**À compter du 30 juin 2020,** nous n’ajouterons plus de nouvelles fonctionnalités à ADAL et Azure AD Graph. Nous continuerons à fournir un support technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.

À compter **du 30 juin 2022,** nous arrêterons la prise en charge d’ADAL et d’Azure AD Graph et ne fournirons plus de support technique ni de mises à jour de sécurité.

Les applications utilisant ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais n’auront pas de support technique ou de mises à jour de sécurité.

Les applications utilisant Azure AD Graph après cette période peuvent ne plus recevoir de réponses du point de terminaison Azure AD Graph.

**ADAL Migration**

Nous vous recommandons de mettre à jour la bibliothèque d’authentification [Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)qui dispose des dernières fonctionnalités et mises à jour de sécurité.

Si vous utilisez des applications Microsoft, sachez que Microsoft est en train de migrer ses applications vers MSAL à l’échéance de fin du support, en veillant à ce qu’elles bénéficient des améliorations constantes de la sécurité et des fonctionnalités de MSAL.

1. [Lisez le FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Découvrez comment migrer des applications par plateforme.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Si vous avez besoin d’aide pour savoir quelles applications utilisent ADAL, nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, d’atteindre les fournisseurs de logiciels indépendants ou les fournisseurs d’applications. Le support Microsoft peut également vous fournir une liste de toutes les applications non-Microsoft ADAL de votre client.

**AAD Graph Migration**

Pour les applications qui utilisent Azure AD Graph, suivez nos instructions pour migrer des applications [Azure AD Graph vers Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Notre liste de contrôle de migration fournit un point de départ.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Votre portail d’inscription d’application Azure indique les applications qui utilisent AAD Graph. Nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, de joindre des fournisseurs de logiciels indépendants ou des fournisseurs d’applications. Le support Microsoft peut également vous fournir une liste de toutes les utilisations d’AAD Graph dans votre client.
1. Pour que votre application puisse accéder aux données dans Microsoft Graph, l’utilisateur ou l’administrateur doivent lui accorder les autorisations appropriées via un processus de consentement. La [référence des autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) répertorie les autorisations associées à chaque ensemble majeur d’API Microsoft Graph. Elle fournit également des instructions sur l’utilisation des autorisations.
