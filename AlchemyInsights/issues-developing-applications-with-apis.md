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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013458"
---
# <a name="issues-developing-applications-with-apis"></a>Problèmes de développement d’applications avec des API

Pour commencer à utiliser l’API Azure Active Directory Graph, consultez le guide de démarrage rapide de [l’API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ou consultez la documentation interactive de référence de l’API Azure [AD Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Fin de la prise en charge de Azure Active Directory Authentication Library (ADAL) et de l’API Azure AD Graph (AAD Graph)**

**À compter du 30 juin 2020,** nous n’ajouterons plus de nouvelles fonctionnalités à ADAL et Azure AD Graph. Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.

À compter du **30 juin 2022,** nous arrêterons la prise en charge d’ADAL et d’Azure AD Graph et ne fournirons plus de support technique ni de mises à jour de sécurité.

Les applications qui utilisent ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais ne bénéficieront pas d’un quelconque support technique ni de mises à jour de sécurité.

Les applications utilisant Azure AD Graph après cette période risquent de ne plus recevoir de réponses du point de terminaison AAD Graph.

**Migration de la Bibliothèque d'authentification Active Directory (ADAL)**

Nous vous recommandons d’effectuer la mise à jour vers la [Bibliothèque d’authentification Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), qui contient les dernières fonctionnalités et mises à jour de sécurité.

Si vous utilisez des applications Microsoft, sachez que Microsoft est en train de migrer ses applications vers MSAL à l’échéance de fin du support, en veillant à ce qu’elles bénéficient des améliorations constantes de la sécurité et des fonctionnalités de MSAL.

1. [Lisez la FAQ sur la bibliothèque ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [En savoir plus sur la migration des applications selon la plateforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Si vous avez besoin d’aide pour savoir quelles applications utilisent ADAL, nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, d’atteindre les fournisseurs de logiciels indépendants ou les fournisseurs d’applications. L’équipe Support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre locataire (tenant).

**Migration des applications AAD Graph**

Pour les applications qui utilisent Azure AD Graph, suivez nos instructions pour migrer les applications [Azure AD Graph vers Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Notre liste de vérification de la migration fournit un point de mise en route](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Votre portail d’inscription d’applications Azure indique les applications qui utilisent AAD Graph. Nous vous recommandons d’examiner le code source de toutes vos applications et, le cas échéant, de faire appel à un éditeur de logiciels ou à un fournisseur d’applications indépendant. Le support Microsoft peut également vous fournir une liste de toutes les utilisations Graph AAD dans votre client.
1. Pour que votre application puisse accéder aux données dans Microsoft Graph, l’utilisateur ou l’administrateur doivent lui accorder les autorisations appropriées via un processus de consentement. La [référence des autorisations Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Microsoft répertorie les autorisations associées à chaque ensemble majeur d’API Graph Microsoft. Elle fournit également des instructions sur l’utilisation des autorisations.
