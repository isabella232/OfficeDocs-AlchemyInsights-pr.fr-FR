---
title: Problèmes avec les liens et les URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707880"
---
# <a name="issues-with-links-and-urls"></a>Problèmes avec les liens et les URL

Les URI de redirection/URLde réponse (les deux expressions sont interchangeables) sont les URL permettant à la Plateforme d’identités Microsoft de renvoyer les jetons demandés par les applications. Si vous souhaitez en savoir plus sur ces URL, veuillez consulter les articles suivants :

- [Flux d’authentification et scénarios d’applications](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) : informations sur les URI de redirection dans la page **Inscription d’application** concernant chaque scénario.
- [Limitations et restrictions des URI de redirection (URL de réponse)](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Je ne sais pas comment inscrire le bon URI de redirection/la bonne URL de réponse pour mon application**

Lorsque vous vous connectez avec l’application en cours de développement, si la boîte de dialogue de configuration affiche **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, vous devez ajouter à votre inscription d’application l’URI de redirection déjà utilisé par votre code utilise dans la demande de jeton d’accès à la Plateforme d’identités Microsoft.

Pour ajouter une URL de réponse, accédez à l’onglet **Authentification** de la page **Inscription d’application** du portail Azure, puis ajoutez une entrée dans la section **URI de redirection**. La valeur à entrer dépend du type d’application en cours de création, comme décrit ci-dessous :

- Pour les applications monopages et les applications web, l’URL de réponse est une URL dans votre application. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Application monopage : Inscription d'application](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ou [Inscrire une application à l’aide du Portail Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Pour les applications de bureau, la valeur à choisir dépend des éléments suivants :
    - plateforme (MacOS est différent de Windows ou Linux)
    - mode d’acquisition du jeton (de manière interactive, par flux de code d’appareil, par authentification Windows intégrée [IWA] ou par nom d’utilisateur/mot de passe).
    Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Application de bureau : Inscription d’application - URI de direction](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Pour les applications mobiles, l’URI de redirection dépend des éléments suivants :
    - plateforme (iOS/Android/UWP)
    - informations permettant de créer votre application, telles que l’ID d’offre groupée dans iOS, et le hachage du nom et de la signature du package sur Android. L’inscription d’une application auprès du Portail Microsoft Azure vous sera utile. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Configuration de la plateforme et URI de redirection](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Les API web et certains modes silencieux d’acquisition des jetons (IWA et nom d’utilisateur/mot de passe) ne nécessitent pas d’URI de redirection.

**J’ai déployé mon application web et, lorsque je teste l’application déployée, je reçois en réponse un message indiquant que l’URL est incompatible**

Ajoutez des URI de redirection à tous les emplacements où vous déployez votre application web. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Inscrire une application web à l’aide du Portail Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Ajoutez l’URI de redirection d’un emplacement immédiatement après avoir déployé l’application à cet emplacement.

**Je ne peux pas inscrire suffisamment d’URL de réponse**

Vous êtes éditeur de logiciels indépendant, et vous disposez d’un ou plusieurs URI de redirection pour chaque client. Vous voulez effectuer une migration d’ADAL/Azure AD v1.0 vers MSAL/la Plateforme d’identités Microsoft, et vous avez atteint le [nombre maximal d’URI de redirection](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Pour résoudre ce problème, [ajoutez des URI de redirection vers les principaux de service](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) correspondant à chacun de vos clients.
