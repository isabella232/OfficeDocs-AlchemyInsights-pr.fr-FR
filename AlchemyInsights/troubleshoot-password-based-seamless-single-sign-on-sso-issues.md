---
title: Résoudre les problèmes DSO (Single Sign-On) transparents basés sur mot de passe
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972822"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Résoudre les problèmes DSO (Single Sign-On) transparents basés sur mot de passe

Pour découvrir les principes de base de l’authentification unique basée sur un mot de passe, consultez l’authentification par mot de passe [avec Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurer l' utilisateur unique basé sur un mot de passe**

1. [Configurer l' sign-on unique](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) basée sur un mot de passe : cet article décrit plus en détail l’option DSO basée sur un mot de passe. Si l’application que vous ajoutez nécessite une configuration personnalisée et que vous devez utiliser l’personnalisation unique basée sur un mot de passe, cet article est à votre place.
2. [Configurez l'](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) connexion unique basée sur un mot de passe pour les applications sur site : le proxy d’application prend en charge plusieurs modes d' connexion unique. L’authentification basée sur un mot de passe est destinée aux applications qui utilisent une combinaison nom d’utilisateur/mot de passe pour l’authentification. Lorsque vous configurez l' sign-on par mot de passe pour votre application, vos utilisateurs doivent se connecter une seule fois à l’application sur site. Après cela, Azure Active Directory stocke les informations de connectez-vous et les fournit automatiquement à l’application lorsque vos utilisateurs y accèdent à distance.
    - Vous devez déjà avoir publié et testé votre application avec le proxy d’application. Si ce n’est pas le cas, suivez les étapes de publication d’applications à l’aide du [proxy d’application Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) puis poursuivez votre configuration de l’sO basée sur un mot de passe pour les applications sur site.

Pour résoudre les problèmes d' ssO basée sur un mot de passe, voir Résoudre les problèmes d' [sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) unique basé sur mot de passe dans Azure AD
