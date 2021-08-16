---
title: Configurer et personnaliser des applications
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044986"
---
# <a name="configure-and-customize-applications"></a>Configurer et personnaliser des applications

**Configurer des applications**

1. Démarrage rapide : la configuration des propriétés d’une application dans votre [client Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vous montre comment configurer certaines propriétés d’une application.
2. Pour vous aider à intégrer vos applications à Azure Active Directory, nous avons développé un [ensemble](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) de didacticiels qui vous guident tout au long de la configuration.
3. [La configuration d’une application proxy d’application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) vous permet de comprendre comment configurer une application proxy d’application dans Azure AD pour exposer vos applications sur site au cloud.
4. Téléchargez [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)et configurez votre application : suivez les instructions de la page Configurer *PingAccess* pour Azure AD pour protéger les applications publiées à l’aide du proxy d’application Microsoft Azure AD sur le site web Ping Identity et téléchargez la dernière version de PingAccess.

**Erreurs d’application mal configurée (AADSTS650056)**

1. Assurez-vous que vous accédez à l’application à partir de l’adresse de connecteur fournie par le propriétaire de l’application. Autrement dit, connectez-vous à l’application par le biais de son processus normal. Dans la plupart des cas, cela se résout automatiquement naturellement. Si ce n’est pas le cas, ce billet peut vous aider à résoudre les problèmes.
2. **Si votre organisation est propriétaire de l’application** (ce qui signifie que l’inscription de l’application se trouve dans votre organisation) :
    - Au minimum, nous vous recommandons d’ajouter l’autorisation déléguée Graph `User.Read` `openid` **Microsoft.**
    - Assurez-vous que l’application et toutes ses autorisations sont consenties. Vous pouvez le vérifier en regardant la colonne **État** de l’inscription de l’application dans **les autorisations d’API.**
    - Dans certains scénarios, l’application peut être tierce, mais elle peut être inscrite dans votre organisation. Confirmez si cette application est répertoriée dans vos inscriptions d’application (pas Enterprise applications).
    - Si vous continuez à voir ce message d’erreur. Ensuite, vous devrez peut-être créer l’URL de consentement décrite à **l’étape 4.**
3. **Si votre organisation n’est pas le propriétaire de l’application et l’utilise en tant qu’application tierce**:
    - Si vous êtes l’administrateur général/d’entreprise, vous devez voir l’écran de consentement. Veillez à cocher la case **« Consentement au nom de votre organisation**».
    - Si vous ne voyez pas l’écran de consentement, supprimez l’application Enterprise et essayez à nouveau.
    - Si vous continuez à voir ce message d’erreur. Ensuite, vous devrez peut-être créer l’URL de consentement décrite à **l’étape 4.**
4. Générez manuellement **l’URL** de consentement à utiliser : si l’application est conçue pour accéder à une ressource spécifique, il se peut que vous ne soyez pas en mesure d’utiliser les boutons de consentement à partir du portail Azure, vous devrez générer manuellement votre propre URL de consentement et l’utiliser.
    - Vous devez obtenir le et `{App-Id}` le du propriétaire de `{App-Uri-Id}` l’application. `{Tenant-Id}` sera votre identificateur client. Il s’ra soit `yourdomain.onmicrosoft.com` de votre ID d’annuaire, soit de votre ID d’annuaire.
    - Si l’application accède à elle-même pour la ressource, le et `{App-Id}` `{App-Uri-Id}` sera identique.
5. Pour plus d’informations, voir Problèmes de se connectant à des applications configurées par [l' sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)unique basée sur SAML.

**Personnaliser les applications**

- Ajoutez une personnalisation à la [page](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) de Azure Active Directory de votre organisation : utilisez le logo et les modèles de couleurs personnalisés de votre organisation pour fournir une apparence cohérente à vos pages de Azure Active Directory (Azure AD).
- [Ajoutez votre nom de domaine personnalisé à l’aide du portail Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - Chaque nouveau client Azure AD est fourni avec un nom de domaine initial. Vous ne pouvez pas modifier ou supprimer le nom de domaine initial, mais vous pouvez ajouter les noms de votre organisation. L’ajout de noms de domaine personnalisés vous permet de créer des noms d’utilisateurs qui sont familiers à vos utilisateurs.
