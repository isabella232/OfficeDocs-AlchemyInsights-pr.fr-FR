---
title: Problèmes avec les jetons
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912004"
---
# <a name="issues-with-tokens"></a>Problèmes avec les jetons

Pour gérer les problèmes liés aux jetons, vous pouvez effectuer ces étapes :

1. Vous pouvez spécifier la durée de vie d’un jeton d’accès, d’ID ou SAML émis par la plateforme d’identités Microsoft. Vous pouvez définir les durées de vie des jetons pour toutes les applications de votre organisation, pour une application mutualisée (multi-organisation) ou pour un principal de service spécifique dans votre organisation. Pour plus d'informations, consultez [Durées de vie des jetons configurables dans la plateforme d'identité de Microsoft (préversion)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Les jetons Access permettent aux clients d’appeler des API web protégées en toute sécurité et sont utilisés par les API web pour effectuer l’authentification et l’autorisation. Comme pour la spécification OAuth, les jetons d’accès sont des chaînes opaques sans format de jeu : certains fournisseurs d’identité (IDPs) utilisent des GUID, tandis que d’autres utilisent des blobs chiffrés. La plateforme d’identité Microsoft utilise différents formats de jeton d’accès, selon la configuration de l’API qui accepte le jeton. Pour découvrir comment votre API peut valider et utiliser les revendications dans un jeton d’accès, consultez [Jetons d’accès de la plateforme d’identité Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. La bibliothèque d’authentification Microsoft (MSAL) prend en charge l’utilisation de plusieurs flux d’authentification dans différents scénarios d’application. Pour plus d’informations, consultez [Flux d’authentification](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. L’autorisation de code d’autorisation OAuth 2.0 peut être utilisée dans les applications installées sur un appareil pour accéder à des ressources protégées, telles que les API web. À l’aide de l’implémentation de la plateforme d’identité Microsoft OAuth 2.0, vous pouvez ajouter l’accès à la connexion et à l’API à vos applications mobiles et de bureau. Consultez [Plateforme d’identité Microsoft et flux de code d’autorisation OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) pour la programmation directe via le protocole dans votre application, en utilisant n’importe quelle langue.
5. OpenID Connect (OIDC) est un protocole d’authentification intégré à OAuth 2.0 que vous pouvez utiliser pour connecter en toute sécurité un utilisateur à une application. Lorsque vous utilisez l’implémentation OpenID Connect du point de terminaison de la plateforme d’identité Microsoft, vous pouvez ajouter un accès de connexion et d’API à vos applications. [La plateforme d’identité Microsoft et le protocole OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) expliquent la procédure indépendamment de la langue et décrit l’envoi et la réception de messages HTTP sans utiliser une bibliothèque Microsoft open source.
    - Le point de terminaison UserInfo fait partie de la norme OIDC, conçue pour renvoyer les réclamations concernant l’utilisateur authentifié. Pour plus d’informations, consultez [Point de terminaison userInfo de la plateforme d’identités Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)
    - L’exemple [Appeler une API web dans une application web à l’aide de Azure AD et OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) montre comment créer une application web MVC qui utilise Azure AD pour se connecter à l’aide du protocole OpenID Connect pour appeler une API web sous l’identité de l’utilisateur connecté à l’aide de jetons obtenus via OAuth 2.0. Cet exemple utilise l’intergiciel OWIN ASP.Net OpenID Connect et ADAL .Net.
6. [Configurer une application pour exposer une API web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - Dans ce démarrage rapide, vous devez inscrire une API web sur la plateforme d’identités Microsoft et l’exposer aux applications clientes en ajoutant une étendue d’exemple. L’inscription et l’exposition de votre API web à travers des étendues, vous permet de fournir un accès basé sur les autorisations à ses ressources aux utilisateurs autorisés et aux applications clientes qui accèdent à votre API.
7. Dans Azure Active Directory B2C (Azure AD B2C), le flux d’identifiants de mot de passe du propriétaire de la ressource (ROPC) est un flux d’authentification standard OAuth. Dans ce flux, une application, également appelée partie fiable, permet d’échanger des identifiants valides pour les jetons. Les identifiants incluent un identifiant d’utilisateur et un mot de passe. Les jetons renvoyés sont un jeton d’ID, un jeton d’accèss et un jeton d’actualisation. Pour plus d’informations, consultez [Configurer un flux d’identifiants de mot de passe de propriétaire de ressource dans Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

