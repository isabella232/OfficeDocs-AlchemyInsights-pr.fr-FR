---
title: Erreurs d’application
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
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976892"
---
# <a name="application-errors"></a>Erreurs d’application

Vous recherchez des informations sur les codes d’erreur **AADSTS** renvoyés par le service d’jetons de sécurité (STS) Azure Active Directory (Azure AD) ? Lisez les codes d’erreur d’authentification et d’autorisation [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pour trouver des descriptions d’erreur, des correctifs et des solutions de contournement AADSTS suggérées.

Les erreurs d’autorisation peuvent être le résultat de plusieurs problèmes différents, dont la plupart génèrent une erreur 401 ou 403. Par exemple, les problèmes suivants peuvent donner lieu à des erreurs d’autorisation :

- [Flux d’acquisition de jetons d’accès](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorrects 
- Mauvaise configuration des [étendues d’autorisations](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Absence de [consentement](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Pour résoudre les erreurs d’autorisation courantes, essayez les étapes ci-dessous qui sont les plus proches de l’erreur que vous recevez. Plusieurs peuvent s’appliquer.

**Erreur (401) Non autorisé : votre jeton est-il valide ?**

Assurez-vous que votre application présente un jeton d’accès valide à Microsoft Graph dans le cadre de la demande. Cette erreur signifie souvent que le jeton d’accès peut être manquant dans l’en-tête de demande d’authentification HTTP ou que le jeton n’est pas valide ou est arrivé à expiration. Nous vous recommandons vivement d’utiliser la [Bibliothèque d’authentification Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) pour l’acquisition des jetons d’accès. En outre, cette erreur peut se produire si vous essayez d’utiliser un jeton d’accès délégué accordé à un compte Microsoft personnel pour accéder à une API qui prend uniquement en charge les comptes scolaires ou de travail (comptes d’organisation).

**Erreur 403 Forbidden : avez-vous choisi le groupe d’autorisations approprié ?**

Vérifiez que vous avez demandé le jeu d’autorisations correct basé sur les API Microsoft Graph que votre application appelle. Les autorisations moins privilégiées recommandées sont fournies dans toutes les rubriques de méthode de référence de l’API Microsoft Graph. Ces autorisations doivent de plus être accordées à l’application par un utilisateur ou un administrateur. L’octroi d’autorisations se produit normalement par l’intermédiaire d’une page de consentement ou par l’octroi d’autorisations en utilisant le panneau d’inscription de l’application sur le portail Azure. Dans le panneau **Paramètres** de l’application, cliquez sur **Autorisations nécessaires**, puis sur **Accorder des autorisations**.

- [Autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Comprendre les autorisations et le consentement d’Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Erreur 403 Forbidden : l’application a-t-elle acquis un jeton correspondant aux autorisations choisies ?**

Vérifiez que le type d’autorisations demandé ou accordé correspond au type de jeton d’accès acquis par votre application. Vous êtes susceptible de demander ou d’accorder des autorisations d’application, mais en utilisant des jetons de flux de codes interactifs délégués au lieu de jetons de flux d’informations d’identification du client, ou en demandant et accordant des autorisations déléguées à l’aide de jetons de flux d’informations d’identification du client au lieu de jetons de flux de codes délégués.

- [Obtenir l’accès au nom des utilisateurs et les autorisations déléguées](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 : flux de codes d’autorisation OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obtenir un accès sans les autorisations de l’utilisateur (service démon) ou de l’application](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 : flux d’informations d’identification du client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Erreur 403 Forbidden : réinitialisation du mot de passe**

Il n’existe à l’heure actuelle aucune autorisation d’application de service à service démon permettant de réinitialiser les mots de passe des utilisateurs. Ces API sont uniquement prises en charge en utilisant le flux de code délégué interactif et un administrateur connecté.

- [Autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Interdit : l’utilisateur a-t-il accès et est-il titulaire d’une licence ?**

Pour les flux de code délégués, Microsoft Graph évalue si la demande est autorisée en fonction des autorisations accordées à l’application et des autorisations dont dispose l’utilisateur. En règle générale, cette erreur indique que l’utilisateur ne dispose pas de privilèges suffisants pour effectuer la demande ou que l’utilisateur ne dispose pas de licence pour l’accès aux données. Seuls les utilisateurs disposant des autorisations ou licences requises peuvent effectuer la demande de manière correcte.

**403 Interdit : avez-vous sélectionné l’API de ressources correcte ?**

Les services d’API tels que Microsoft Graph vérifient que la revendication aud (audience) dans le jeton d’accès reçu correspond à la valeur prévue pour elle-même et, si ce n’est pas le cas, une erreur 403 Forbidden se produit. Une erreur courante résultant de cette erreur est d’essayer d’utiliser un jeton acquis pour les API Azure AD Graph, les API Outlook ou les API SharePoint/OneDrive pour appeler Microsoft Graph (ou vice versa). Assurez-vous que la ressource (ou l’étendue) pour laquelle votre application fait l’acquisition d’un jeton correspond à l’API appelée par l’application.

**400 Demande incorrecte ou 403 Interdit : l’utilisateur satisfait-il aux stratégies d’accès conditionnel (CA) de votre organisation ?**

En fonction des stratégies d’accès client d’une organisation, un utilisateur accédant aux ressources Microsoft Graph via votre application peut être mis à l’épreuve pour obtenir des informations supplémentaires qui ne sont pas présentes dans le jeton d’accès acquis à l’origine par votre application. Dans ce cas, votre application reçoit un 400 avec l’erreur *interaction_required* lors de l’acquisition du jeton d’accès ou un 403 avec l’erreur *insufficient_claims* lorsque vous appelez Microsoft Graph. Dans les deux cas, la réponse d’erreur contient d’autres informations qui peuvent être présentées au point de terminaison autoriser afin de demander des éléments supplémentaires (telles que l’authentification multifacteur ou l’inscription de l’appareil) à l’utilisateur.

- [Gestion des défis liés à l’accès conditionnel à l’aide de MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Conseils aux développeurs pour l’accès conditionnel Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
