---
title: Configurer l' sign-on unique (SSO) transparente
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402265"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurer l' sign-on unique (SSO) transparente

**Configurer des applications**

1. Vous devez obtenir les valeurs du fournisseur de l’application. Vous pouvez entrer manuellement les valeurs ou télécharger un fichier de métadonnées pour extraire la valeur des champs.
2. De nombreuses applications ont déjà été pré-configurées pour fonctionner avec Azure AD. Ces applications sont répertoriées dans la galerie d’applications que vous pouvez parcourir lorsque vous ajoutez une application à votre client Azure AD. La [série de démarrage rapide](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vous dirige tout au long du processus.
3. Pour créer une application non galerie, vous pouvez cliquer sur + Créer votre propre bouton **Application** et donner un nom à votre application.
    - Par défaut, il sélectionne Intégrer toute autre application que vous ne trouvez pas dans la galerie, ce qui est **l’option** correcte pour les applications non-galerie.
    - Une fois que **vous avez atteint Créer** après avoir mis le nom de l’application, il crée une application d’entreprise non galerie.
    - Ensuite, vous pouvez accéder à l' **sign-on** unique sous **Gérer** cette application et vous pourrez voir différentes techniques pour l’implémenter dans votre environnement.

**Configurer l' sso transparente pour une application spécifique**

Pour les applications de la galerie, vous trouverez des instructions détaillées pas à pas. Pour accéder aux étapes, vous pouvez parcourir la liste de tous les didacticiels de configuration d’application dans [les didascticiels](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)de configuration d’application SaaS.

**Configurer l’pertinence basée sur SAML**

1. Démarrage rapide : configurer l' [sign-on saml (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)pour une application dans votre client Azure Active Directory (Azure AD).
2. Pour en savoir plus sur l’option SAML pour l' sign-on unique, voir Comprendre l' [sign-on basée sur SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Pour en savoir plus sur les demandes d’authentification SAML 2.0 et les réponses qu’Azure Active Directory (Azure AD) prend en charge pour l’authentification unique Sign-On (SSO), consultez le protocole SAML Sign-On [single-Sign-On.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Pour découvrir comment créer et configurer une connexion unique basée sur SAML pour votre application dans Azure Active Directory (Azure AD) à l’aide de l’API Microsoft Graph, voir Configurer l' connexion unique basée sur SAML pour votre application à l’aide de [l’API Microsoft Graph.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Pour découvrir comment Azure AD utilise le protocole SAML, voir comment la plateforme d’identités [Microsoft utilise le protocole SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Configurer les jetons et les revendications**

1. [How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Pour savoir comment configurer des revendications à l’aide de PowerShell, voir How [to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Pour savoir comment configurer des revendications facultatives, voir Comment : fournir des revendications [facultatives à votre application.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Pour apprendre à utiliser les attributs d’extension de schéma d’annuaire pour envoyer des données utilisateur à des applications dans des revendications de jeton, voir Utilisation des [attributs d’extension](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)de schéma d’annuaire dans les revendications.
5. Pour savoir comment configurer les durées de vie des jetons, voir Durées de vie des jetons configurables dans la plateforme [d’identités Microsoft (prévisualisation).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. Configurer des stratégies de durée de vie de jeton [(prévisualisation)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) : dans cet article, nous allons passer en revue un scénario de stratégie commun qui peut vous aider à imposer de nouvelles règles pour la durée de vie des jetons. Dans l’exemple, vous allez apprendre à créer une stratégie qui oblige les utilisateurs à s’authentifier plus fréquemment dans votre application web.

**Résoudre les problèmes de configuration de l’oD SSO**

- Pour les questions fréquemment posées sur azure Active Directory seamless single Sign-On (Seamless SSO), voir [Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Pour obtenir des informations de dépannage sur les problèmes courants liés à la Sign-On unique transparente Azure Active Directory (Azure AD), voir Résoudre les problèmes liés à l' [sign-on transparente Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
