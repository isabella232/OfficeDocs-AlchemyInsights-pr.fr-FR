---
title: Problèmes de connexion ssO
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084344"
---
# <a name="sso-connection-issues"></a>Problèmes de connexion ssO

1. Suivez le guide[Démarrage rapide : configurez les propriétés d’une application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) pour configurer votre application.
2. En fonction de l’application et [de l’option d' sign-on unique](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que vous avez choisies, suivez les instructions appropriées ci-dessous :
    - Pour configurer une **application** sur site pour l' **sign-on saml** unique, voir [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Pour configurer une **application cloud pour** l' **sign-on unique** basée sur un mot de passe, voir Configurer l'  [sign-on unique de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)mot de passe.
    - Pour configurer une **application** sur site pour l' **sign-on** unique via le proxy d’application, voir Coffre de mots de passe pour l' [sign-on unique avec le proxy d’application.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Résolution** des problèmes de proxy d’application : nous vous recommandons de commencer par passer en revue le flux de dépannage, déboguer les problèmes du connecteur de [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)d’application, pour déterminer si les connecteurs proxy d’application sont configurés correctement. Si vous avez encore des difficultés pour vous connecter à l’application, suivez le flux de dépannage dans déboguer les problèmes de [l’application proxy d’application.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Vous pouvez identifier [les problèmes CORS à l’aide](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) des outils de débogage du navigateur :
    - Lancez le navigateur et naviguez jusqu'à l'application web.
    - Appuyez sur **F12** pour faire apparaître la console de débogage.
    - Essayez de reproduire la transaction et examinez le message de la console. Une violation du CORS produit une erreur de console sur l'origine.
    - Certains problèmes CORS ne peuvent pas être résolus, par exemple lorsque votre application redirige vers login.microsoft.com pour s’authentifier et que le jeton d’accès expire. L’appel CORS échoue ensuite. Une solution de contournement pour ce scénario consiste à prolonger la durée de vie du jeton d'accès, pour éviter qu'il n'expire pendant la session d'un utilisateur. Pour plus d'informations sur la manière de procéder, voir [Durée de vie des jetons configurables dans la plate-forme d'identité de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Résolution des problèmes liés à l' **sign-on** unique saml : nous vous recommandons de vérifier les problèmes de se connectant aux applications [saml](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)configurées pour trouver les solutions aux problèmes que vous êtes le plus susceptible de rencontrer.
5. Résolution des problèmes d' **sign-on** unique basé sur mot de passe : nous vous recommandons de vérifier la résolution des problèmes d' [sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)unique basé sur mot de passe dans Azure AD , pour trouver les solutions aux problèmes que vous êtes le plus susceptible de rencontrer.
6. Pour les problèmes de connexion lors de l’utilisation d’un VPN, voir Comment utiliser l' signature unique [(SSO) sur VPN et Wi-Fi connexions.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
