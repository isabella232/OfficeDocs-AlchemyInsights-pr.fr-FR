---
title: Résoudre les problèmes d’OIDC (Single Sign-on) transparent (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726920"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Résoudre les problèmes d’OIDC (Single Sign-on) transparent (SSO)

- Pour découvrir comment ajouter une application basée sur OIDC à votre client Azure, voir Démarrage rapide : configurer l' utilisateur unique basé sur OIDC pour une application dans votre client [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Pour plus d’informations sur les applications qui utilisent la norme OpenID Connect pour implémenter l’ouvrez-vous, voir Comprendre l’ouvrez-vous à [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Pour plus d’informations au cas où vous choisiriez d’écrire votre code en envoyant et en manipulant directement des demandes HTTP ou en utilisant une bibliothèque open source tierce, plutôt que d’utiliser l’une de nos bibliothèques open source, voir [les protocoles OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)et OpenID Connect sur la plateforme d’identités Microsoft.

**Protocoles**

1. Plateforme d’identité [Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) et flux d’octroi implicite : la caractéristique de définition de l’octroi implicite est que les jetons (jetons d’ID ou jetons d’accès) sont renvoyés directement à partir du point de terminaison /authorize au lieu du point de terminaison /token. Il est souvent utilisé dans le cadre du flux de code d’autorisation, dans ce que l’on appelle le « flux hybride », en récupérant le jeton **d’ID** sur la demande /authorize avec un code d’autorisation. Cet article explique comment programmer directement sur le protocole de votre application pour demander des jetons à Azure AD.
2. Plateforme d’identité Microsoft et flux de code d’autorisation [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) : l’octroi de code d’autorisation OAuth 2.0 peut être utilisé dans les applications installées sur un appareil pour accéder aux ressources protégées, telles que les API web. À l’aide de l’implémentation de la plateforme d’identités Microsoft d’OAuth 2.0, vous pouvez ajouter la connexion et l’accès API à vos applications **mobiles et de bureau.** Cet article explique comment programmer directement sur le protocole dans votre application à l’aide de n’importe quel langage.
3. [Plateforme d’identités Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) et protocole OpenID Connect : lorsque vous utilisez l’implémentation de la plateforme d’identités Microsoft OpenID Connect, vous pouvez ajouter une connexion et un accès API à vos applications. Cet article explique comment le faire indépendamment de la langue et explique comment envoyer et recevoir des messages HTTP sans utiliser de bibliothèques **Microsoft open source.**
4. Plateforme d’identité Microsoft et flux d’informations d’identification du [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) : vous pouvez utiliser l’octroi d’informations d’identification client OAuth 2.0 spécifié dans la RFC 6749, parfois appelé **OAuth** à deuxggs, pour accéder aux ressources hébergées sur le web à l’aide de l’identité d’une application. Ce type d’octroi est couramment utilisé pour les interactions de serveur à serveur qui doivent s’exécuter en arrière-plan, sans interaction immédiate avec un utilisateur. Ces types d’applications sont souvent appelés des **daemons** ou des comptes **de service.** Cet article explique comment programmer directement par rapport au protocole dans votre application.
