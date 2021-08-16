---
title: Problèmes avec les bibliothèques d’authentification
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028002"
---
# <a name="issues-with-authentication-libraries"></a>Problèmes avec les bibliothèques d’authentification

1. [Plateforme d’identités Microsoft bibliothèques d’authentification](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) répertorie les bibliothèques clientes et intermédiaires compatibles et compatibles avec Microsoft.
2. La bibliothèque d’authentification Microsoft (MSAL) prend en charge plusieurs flux [d’authentification](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pour une utilisation dans différents scénarios d’application.
3. Pour authentifier et acquérir des jetons, vous initialisez une nouvelle application cliente publique ou confidentielle dans votre code. Vous pouvez définir plusieurs options de configuration lors de l’initialisation de l’application cliente dans la bibliothèque d’authentification Microsoft (MSAL). Pour en savoir plus, consultez les [options de configuration de l’application.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Fin de la prise en charge de Azure Active Directory Authentication Library (ADAL) et de l’API Azure AD Graph (AAD Graph)**

**À compter du 30 juin 2020,** nous n’ajouterons plus de nouvelles fonctionnalités à ADAL et Azure AD Graph. Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.

À compter du **30 juin 2022,** nous arrêterons la prise en charge d’ADAL et d’Azure AD Graph et ne fournirons plus de support technique ni de mises à jour de sécurité.

Les applications qui utilisent ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais ne *bénéficieront pas d’un quelconque support technique ni de mises à jour de sécurité*.

Les applications utilisant Azure AD Graph après cette période risquent de ne plus recevoir de réponses du point de terminaison AAD Graph.

**Migration de la Bibliothèque d'authentification Active Directory (ADAL)**

Nous vous recommandons d’effectuer la mise à jour vers la [Bibliothèque d’authentification Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), qui contient les dernières fonctionnalités et mises à jour de sécurité.

Si vous utilisez des applications Microsoft, sachez que Microsoft est en train de migrer ses applications vers MSAL à l’échéance de fin du support, en veillant à ce qu’elles bénéficient des améliorations constantes de la sécurité et des fonctionnalités de MSAL.

Pour plus d’informations, voir :

1. [Lisez la FAQ sur la bibliothèque ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [En savoir plus sur la migration des applications selon la plateforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Si vous avez besoin d’aide pour savoir quelles applications utilisent ADAL, nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, d’atteindre les fournisseurs de logiciels indépendants ou les fournisseurs d’applications. L’équipe Support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre locataire (tenant).

**Migration des applications AAD Graph**

Pour les applications qui utilisent Azure AD Graph, suivez nos instructions pour migrer les applications [Azure AD Graph vers Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Notre liste de contrôle de migration fournit un point de départ.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Votre portail d’inscription d’applications Azure indique les applications qui utilisent AAD Graph. Nous vous recommandons d’examiner le code source de toutes vos applications et, le cas échéant, de faire appel à un éditeur de logiciels ou à un fournisseur d’applications indépendant. Le support Microsoft peut également vous fournir une liste de toutes les utilisations Graph AAD dans votre client.
3. Pour que votre application puisse accéder aux données dans Microsoft Graph, l’utilisateur ou l’administrateur doivent lui accorder les autorisations appropriées via un processus de consentement. La [référence des autorisations Graph](https://docs.microsoft.com/graph/permissions-reference) Microsoft répertorie les autorisations associées à chaque ensemble majeur d’API Graph Microsoft. Elle fournit également des instructions sur l’utilisation des autorisations.
