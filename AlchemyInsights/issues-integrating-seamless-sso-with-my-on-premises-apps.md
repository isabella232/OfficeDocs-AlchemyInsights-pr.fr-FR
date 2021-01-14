---
title: Problèmes d’intégration de l' sso transparente à mes applications sur site
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848772"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problèmes d’intégration de l' sso transparente à mes applications sur site

Pour résoudre les problèmes d’intégration de l' ssO transparente avec des applications sur site, faites les choses suivantes :

**Étapes recommandées**

1. Pour configurer une **application** sur site pour l' **sign-on** unique via le proxy d’application, voir Coffre de mots de passe pour l' [sign-on unique avec le proxy d’application.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Résolution** des problèmes de proxy d’application : nous vous recommandons de commencer par passer en revue le flux de dépannage, déboguer les problèmes de connecteur de [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)d’application, pour déterminer si les connecteurs proxy d’application sont configurés correctement. Si vous avez encore des difficultés pour vous connecter à l’application, suivez les étapes de résolution des problèmes dans Déboguer les problèmes de [l’application proxy d’application.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Vous pouvez identifier [les problèmes CORS à l’aide](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) des outils de débogage de navigateur suivants :
    1. Lancez le navigateur et accédez à l’application web.
    1. Appuyez **sur F12** pour faire monter la console de débogage.
    1. Essayez de reproduire la transaction et examinez le message de la console. Une violation CORS produit une erreur de console sur l’origine.
    1. Certains problèmes CORS ne peuvent pas être résolus, par exemple lorsque votre application redirige vers login.microsoftonline.com pour s’authentifier et que le jeton d’accès expire. L’appel CORS échoue ensuite. Une solution de contournement pour ce scénario consiste à prolonger la durée de vie du jeton d’accès afin d’éviter qu’il n’arrive à expiration pendant la session d’un utilisateur. Pour plus d’informations sur la façon de faire, voir Durées de vie des jetons [configurables dans la plateforme d’identité Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Documents recommandés**

- [Comment configurer l' sign-on unique sur une application proxy d’application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Sign-on unique SAML pour les applications sur site avec le proxy d’application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Comprendre et résoudre les problèmes CORS du proxy d’application Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Résoudre les problèmes de configuration de délégation Kerberos contrainte pour le proxy d’application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)