---
title: Problèmes de connectez-vous de l’utilisateur de l' signer de façon transparente
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919201"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problèmes de connectez-vous de l’utilisateur de l' signer de façon transparente

Une fois l’utilisateur authentifié, le navigateur met en cache les informations d’identification de l’utilisateur, de sorte que sur le même navigateur, l’application se connecte automatiquement avec le même compte. Cela peut rendre difficile pour un autre utilisateur ou un seul utilisateur de se connecter à plusieurs comptes sur un seul appareil. Pour résoudre ce problème : 1. Essayez de vous inscrire sur un autre navigateur. 2. Clear the browser’s cache and/or cookies and try signing in again.

Si vous rencontrez toujours des problèmes de connectez-vous, nous vous recommandons les étapes suivantes pour diagnostiquer et automatiser les étapes de résolution :

1. Installez [l’extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) de navigateur sécurisé Mes applications pour aider Azure Active Directory (Azure AD) à fournir de meilleurs diagnostics et résolutions lors de l’utilisation de l’expérience de test dans le portail Azure.
2. Reproduisez l’erreur à l’aide de l’expérience de test dans la page de configuration de l’application dans le portail Azure. Pour plus d’informations, voir [Déboguer des applications d' sign-on unique basées sur SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Si vous utilisez l’expérience de test dans le portail Azure avec l’extension de navigateur sécurisé Mes applications, vous pouvez ignorer **l’étape 4.**
4. Pour ouvrir la page de configuration basée sur l’ouvrez-vous unique SAML :
    - Ouvrez [le portail Azure et](https://portal.azure.com/) connectez-vous en tant **qu’administrateur général** ou **coadmin.**
    - Ouvrez **l’extension Azure Active Directory** en sélectionnant Tous les **services** en haut du menu de navigation gauche principal.
    - Tapez « Azure Active Directory » dans la zone de recherche de filtre et sélectionnez **l’élément Azure Active Directory.**
    - Sélectionnez **Applications d’entreprise** dans le menu de navigation gauche d’Azure Active Directory.
    - Sélectionnez **Toutes les applications** pour afficher la liste de toutes vos applications. Si vous ne voyez pas l’application que  vous souhaitez afficher ici, utilisez le contrôle Filtre en haut de la liste Toutes les **applications** et définissez l’option  Afficher sur Toutes les **applications.**
    - Sélectionnez l’application que vous souhaitez configurer pour l' sign-on unique.
    - Après le chargement de l’application, **sélectionnez Sign-on unique** dans le menu de navigation gauche de l’application.
    - Sélectionnez **l' sso saml.**
5. En fonction de l’erreur, pour en savoir plus sur les étapes recommandées à suivre, voir Problèmes de se connectant à des applications d' sign-on unique basées sur [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Pour résoudre d’autres problèmes de signature utilisateur, reportez-vous aux instructions suivantes :
    - [Protocole SAML à Sign-On unique](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Procédure : résoudre les erreurs de sign-in à l’aide des rapports Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Invite de consentement inattendue](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Erreur de consentement de l’utilisateur](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problèmes de signature à partir de Mes applications](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Erreur sur la page de la signature de l’application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problème de signature dans une application Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
