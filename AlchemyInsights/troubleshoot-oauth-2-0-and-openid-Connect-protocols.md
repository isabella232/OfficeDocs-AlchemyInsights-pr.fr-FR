---
title: Résoudre des problèmes des protocoles OAuth 2.0 et OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921041"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Résoudre des problèmes des protocoles OAuth 2.0 et OpenID Connect

Pour résoudre les problèmes d’OAuth 2.0 et d’OpenID Connect, effectuez les étapes recommandées suivantes :

Consultez les articles suivants relatifs à la configuration et la résolution des problèmes liés aux protocoles OAuth 2.0 et OpenID Connect :

- [Plateforme d’identité Microsoft et flux de code d’autorisation OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Cet article décrit comment appliquer des programmes directement contre le **flux d'autorisation de code (PKCE)** dans votre application, en utilisant n'importe quel langage.
- [Plateforme d’identité Microsoft et flux d’informations d’identification du client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Cet article décrit comment appliquer des programmes directement à partir du **flux d’informations d’identification du client** dans votre application.
- [Plateforme d’identité Microsoft et informations d’identification de mot de passe du propriétaire des ressources OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - Cet article décrit comment appliquer un programme directement à partir du **flux ROPC** dans votre application.
    - La plateforme d’identité Microsoft prend uniquement en charge la fonctionnalité ROPC pour les clients Azure AD, et non pour les comptes personnels. Cela signifie que vous devez utiliser un point de terminaison spécifique du client **(https://login.microsoftonline.com/{TenantId_or_Name})** ou le point de terminaison des **organisations**.
    - Les comptes personnels invités à utiliser un client Azure AD ne peuvent pas utiliser la fonctionnalité ROPC.
    - Les comptes qui n’ont pas de mot de passe ne peuvent pas se connecter via la gestion de la sécurité des utilisateurs. Dans ce scénario, nous vous recommandons plutôt d’utiliser un autre flux pour votre application.
    - Si les utilisateurs doivent utiliser l’[authentification multifacteur (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) pour se connecter à l’application, ils seront bloqués.
    - La fonction ROPC n’est pas prise en charge dans les scénarios de [fédération d’identité hybride](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (par exemple, Azure AD et ADFS utilisés pour authentifier des comptes locaux). Si les utilisateurs sont redirigés vers un fournisseur d’identité local, Azure AD ne peut pas tester le nom d’utilisateur et le mot de passe de ce fournisseur d’identité. [Authentification directe](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) est pris en charge avec la fonction ROPC.
    - Une exception à un scénario de fédération d’identité hybride est la suivante : la stratégie de découverte du domaine d’accueil avec **AllowCloudPasswordValidation** définie sur **TRUE** permet au flux ROPC de fonctionner pour les utilisateurs fédérés lorsque les mots de passe locaux sont synchronisés avec le cloud. Pour plus d’informations, consultez [Activer l'authentification directe par ROPC des utilisateurs fédérés pour les applications existantes](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Plateforme d'identité Microsoft et flux On-Behalf-Of OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) : cet article décrit comment appliquer des programmes directement au **flux On-Behalf-Of (OBO)** dans votre application.
- [Plateforme d’identité Microsoft et protocole OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) : cet article explique comment implémenter le protocole OpenID Connect indépendamment de la langue, et décrit comment envoyer et recevoir des messages HTTP sans utiliser de bibliothèques Microsoft open source.

**Jetons d’accès**

[Les jetons d’accès à la plateforme d’identité Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) : Découvrez comment votre API peut valider et utiliser les revendications dans un jeton d’accès. Toute la documentation de cet article, sauf dans le cas indiqué, s’applique uniquement aux jetons émis pour les API que vous avez enregistrées. Elle ne s'applique pas aux jetons émis pour les API appartenant à Microsoft, et ces jetons ne peuvent pas non plus être utilisés pour valider la manière dont la plateforme d'identité Microsoft émettra des jetons pour une API que vous créez.

**Configuration de l’application**

[Restrictions et limitations relatives à l’URI de redirection (URL de réponse)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) : Découvrez comment configurer votre url de redirection URI (URL de réponse). Une URI de redirection, ou URL de réponse, est l’emplacement où le serveur d’autorisation envoie l’utilisateur une fois l’application autorisée et accordé un code d’autorisation ou un jeton d’accès. Le serveur d’autorisation envoie le code ou le jeton à la redirection de l’URI. Il est donc important que vous enregistriez l’emplacement correct dans le cadre du processus d’inscription de l’application.

**Mise en service des applications**

[Didacticiel : développer et planifier l’approvisionnement d'un point de terminaison SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - Cet article décrit comment créer un point de terminaison SCIM et intégrer ce dernier au service d’approvisionnement AAD.


