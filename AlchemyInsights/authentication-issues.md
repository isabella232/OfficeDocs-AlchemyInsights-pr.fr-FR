---
title: Problèmes d’authentification
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
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976847"
---
# <a name="authentication-issues"></a>Problèmes d’authentification

**Recherchez-vous des informations sur les codes d’erreur AADSTS renvoyés depuis le service d'émission de jeton de sécurité Azure Active Directory (Azure AD) ?** Veuillez consulter la page [Codes d’erreur d’authentification et d’autorisation Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pour trouver les descriptions des erreurs AADSTS, les correctifs et certaines solutions de contournement recommandées.

Les erreurs d’autorisation peuvent provenir de toutes sortes de problèmes, dont la plupart génèrent une erreur 401 ou 403. Par exemple, les problèmes suivants peuvent donner lieu à des erreurs d’autorisation :

- [Flux d’acquisition de jetons d’accès](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorrects 
- Mauvaise configuration des [étendues d’autorisations](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Absence de [consentement](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Les procédures suivantes permettent de résoudre les erreurs d’autorisation les plus courantes. Veuillez suivre celle correspondant le mieux à l’erreur que vous rencontrez. Plusieurs procédures peuvent s’appliquer à l’erreur que vous rencontrez.

**Erreur « 401 Unauthorized » (« Non autorisé ») : votre jeton est-il valide ?**

Vérifiez que votre application présente un jeton d’accès valide à Microsoft Graph lors de la demande. Cette erreur signifie souvent que le jeton d’accès ne figure pas dans l’en-tête de demande d’authentification HTTP, que le jeton n’est pas valide ou qu’il est arrivé à expiration. Nous vous recommandons vivement d’utiliser la Bibliothèque d’authentification Microsoft (MSAL) pour l’acquisition des jetons d’accès. En outre, cette erreur peut se produire si vous essayez d’utiliser un jeton d’accès délégué accordé à un compte Microsoft personnel pour accéder à une API prenant uniquement en charge les comptes professionnels ou scolaires (comptes d’organisation).

**Erreur « 403 Forbidden » (« Interdit ») : avez-vous choisi le groupe d’autorisations approprié ?**

Vérifiez que vous avez demandé le jeu d’autorisations adapté aux API Microsoft Graph appelées par votre application. Les autorisations de droit d’accès minimal recommandées figurent dans toutes les rubriques sur la méthode de référence de l’API Microsoft Graph. De plus, un utilisateur ou un administrateur doit accorder ces autorisations à l’application. L’octroi d’autorisations se produit normalement via une page de consentement ou à l’aide du panneau d’inscription de l’application sur le Portail Azure. Dans le panneau **Paramètres** de l’application, cliquez sur **Autorisations nécessaires**, puis sur **Accorder des autorisations**. Si vous souhaitez en savoir plus, veuillez consulter ces pages :

- [Autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Comprendre les autorisations et le consentement d’Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Erreur « 403 Forbidden » (« Interdit ») : l’application a-t-elle acquis un jeton correspondant aux autorisations choisies ?**

Vérifiez que les types d’autorisations demandées ou accordées correspondent au type de jeton d’accès acquis par votre application. En effet, nul n’est à l’abri d’une erreur. Par exemple, lors d’une demande ou d’un octroi d’autorisations pour une application, il y a toujours un risque de confondre des jetons de flux de codes interactifs délégués avec des jetons de flux d’informations d’identification client, ou l’inverse.

Si vous souhaitez en savoir plus sur l’obtention de jetons, veuillez consulter les rubriques suivantes :

- [Obtenir l’accès au nom des utilisateurs et les autorisations déléguées](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 : flux de codes d’autorisation OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obtenir un accès sans les autorisations de l’utilisateur (service démon) ou de l’application](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 : flux d’informations d’identification du client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Erreur « 403 Forbidden » (« Interdit ») : réinitialisation du mot de passe**

Il n’existe à l’heure actuelle aucune autorisation d’application de service à service démon permettant de réinitialiser les mots de passe des utilisateurs. Ces API sont uniquement prises en charge en utilisant le flux de code délégué interactif et un administrateur connecté. Si vous souhaitez en savoir plus, veuillez consulter la page [Référence des autorisations de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**Erreur « 403 Forbidden » (« Interdit ») : l’utilisateur dispose-t-il des droits d’accès adéquats et est-il titulaire d’une licence ?**

Pour les flux de code délégués, Microsoft Graph évalue si la demande a été autorisée sur la base des autorisations accordées à l’application et des autorisations de l’utilisateur connecté. En règle générale, cette erreur indique que l’utilisateur ne dispose pas de privilèges suffisants pour effectuer la demande **ou** que l’utilisateur ne dispose pas de licence pour l’accès aux données. Seuls les utilisateurs disposant des autorisations ou licences requises peuvent effectuer la demande de manière correcte.

**Erreur « 403 Forbidden » (« Interdit ») : avez-vous sélectionné l’API de ressources adéquate ?**

Les services API tels que Microsoft Graph vérifient que la revendication *aud* (audience) du jeton d’accès reçu correspond à la valeur qu’il attend pour lui-même. Si ce n’est pas le cas, une erreur « 403 Forbidden » (« Interdit ») se produit. Généralement, cette erreur peut survenir si vous essayez d’appeler Microsoft Graph en utilisant un jeton acquis pour les API Azure AD Graph, les API Outlook ou les API SharePoint/OneDrive. Assurez-vous que la ressource (ou l’étendue) pour laquelle votre application fait l’acquisition d’un jeton correspond à l’API appelée par l’application.

**Erreur « 400 Bad Request » (« Requête incorrecte » ou erreur « 403 Forbidden » « Interdit » : l’utilisateur satisfait-il aux stratégies d’accès conditionnel de votre organisation ?**

Les stratégies d’accès conditionnel d’une organisation peuvent exiger qu’un utilisateur accédant aux ressources Microsoft Graph via votre application doive fournir des informations supplémentaires qui n’apparaissent pas dans le jeton d’accès que votre application a acquis au départ. Si l’utilisateur ne respecte pas ces exigences, votre application reçoit une erreur **400 précisant *interaction_required*** lors de l’acquisition du jeton d’accès ou une erreur **403 précisant *insufficient_claims*** lors de l’appel de Microsoft Graph. Dans les deux cas, le message d’erreur reçu contient d’autres informations éventuellement présentées au point de terminaison autorisé, afin de demander des informations ou des actions supplémentaires à l’utilisateur (telles que l’usage de l’authentification multifacteur ou l’inscription de l’appareil).

Si vous souhaitez en savoir plus sur l’accès conditionnel, veuillez consulter les rubriques suivantes :

- [Gérer les challenges d’accès conditionnel à l’aide de la Bibliothèque d’authentification Microsoft](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Conseils aux développeurs pour l’accès conditionnel Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Fin du support de la Bibliothèque d'authentification Active Directory (ADAL) et de l’API Azure AD Graph (AAD Graph)_* _

- À compter du 30 juin 2020, nous n’ajouterons plus de nouvelles fonctionnalités à la Bibliothèque d'authentification Active Directory (ADAL) et à l’API Azure AD Graph (AAD Graph). Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.
- À compter du 30 juin 2022, nous allons mettre fin au support destiné à ADAL et AAD Graph ; nous ne fournirons plus de support technique ni de mises à jour de sécurité.
    - Les applications qui utilisent ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais ne bénéficieront pas d’un quelconque support technique ni de mises à jour de sécurité.
    - Les applications utilisant Azure AD Graph après cette période risquent de ne plus recevoir de réponses du point de terminaison AAD Graph.

_ *Migration de la Bibliothèque d'authentification Active Directory (ADAL)**

Nous vous recommandons d’effectuer la mise à jour vers la [Bibliothèque d’authentification Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), qui contient les dernières fonctionnalités et mises à jour de sécurité. Nous émettons cette recommandation dans le contexte suivant : Microsoft migre ses applications vers la bibliothèque MSAL avant la fin du support technique. La migration, par Microsoft, de ses applications vers la bibliothèque MSAL a pour but de garantir que les applications bénéficient des améliorations constantes apportées par cette bibliothèque en matière de sécurité et de fonctionnalités.

- [Lisez la FAQ sur la bibliothèque ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [En savoir plus sur la migration des applications selon la plateforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Pour savoir si l’une de vos applications utilise ADAL, vous pouvez examiner son code source puis, le cas échéant, faire appel à un éditeur de logiciels ou à un fournisseur d’applications indépendant. L’équipe Support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre locataire (tenant).

**Migration des applications AAD Graph**

Veuillez suivre nos recommandations pour [migrer les applications AAD Graph vers Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Notre liste de vérification de la migration fournit un point de mise en route](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Votre portail d’inscription d’applications Azure indique les applications qui utilisent AAD Graph. Nous vous recommandons d’examiner le code source de toutes vos applications et, le cas échéant, de faire appel à un éditeur de logiciels ou à un fournisseur d’applications indépendant. L’équipe Support Microsoft peut également vous fournir les informations sur la façon dont AAD Graph est utilisé dans votre locataire (tenant).

 










