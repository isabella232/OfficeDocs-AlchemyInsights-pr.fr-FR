---
title: Fonctionnement des bibliothèques d’authentification
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
- "9775"
- "9004342"
ms.openlocfilehash: b667e699e1595b21d80788123de13daffbe79a35b1671e9d35eaa6cd980693db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083084"
---
# <a name="working-with-authentication-libraries"></a>Fonctionnement des bibliothèques d’authentification

Pour résoudre le problème de bibliothèque d’authentification Microsoft (MSAL), effectuez les étapes recommandées suivantes :

1. **Utilisation de MSAL** : [bibliothèques d’authentification de la Plateforme d’identité Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - Cet article présente la prise en charge de la bibliothèque d’authentification Microsoft pour plusieurs types d’applications. Il inclut des liens vers le code source de la bibliothèque. où obtenir le package pour le projet de votre application ; et indique si la bibliothèque prend en charge la connexion de l'utilisateur (authentification), l'accès aux API web protégées (autorisation), ou les deux.

2. **Résolution des problèmes d’authentification** : MSAL prend en charge plusieurs flux d’authentification pour une utilisation dans différents scénarios d’application. Selon la manière dont votre application cliente est conçue, la technologie MSAL peut utiliser un ou plusieurs flux d’authentification pris en charge par la plateforme d’identité Microsoft. Ces flux peuvent produire plusieurs types de jetons et codes d’autorisation, et nécessitent des jetons différents pour les faire fonctionner.

3. **Jetons d’accès** : [Jeton d’accès de la plateforme d’identités Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Découvrez comment votre API peut valider et utiliser les revendications dans un jeton d’accès. Toute la documentation de cet article, sauf dans le cas indiqué, s’applique uniquement aux jetons émis pour les API que vous avez enregistrées. Elle ne s'applique pas aux jetons émis pour les API appartenant à Microsoft, et ces jetons ne peuvent pas non plus être utilisés pour valider la manière dont la plateforme d'identité Microsoft émettra des jetons pour une API que vous créez.

**Fin de la prise en charge de la Bibliothèque d’authentification Azure Active Directory (ADAL)**

- **À compter du 30 juin 2020,** nous n’ajouterons plus de nouvelles fonctionnalités à la Bibliothèque d'authentification Active Directory (ADAL) et à l’API Azure AD Graph (AAD Graph). Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.
- **À compter du 30 juin 2022,** nous allons mettre fin à l'assistance pour ADAL et Azure AD Graph et ne fournirons plus d'assistance technique ni de mises à jour de sécurité.
- Les applications qui utilisent ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais ne *bénéficieront pas d’un quelconque support technique ni de mises à jour de sécurité*.
- Les applications utilisant Azure AD Graph après cette période risquent de ne plus recevoir de réponses du point de terminaison AAD Graph.

**Migration de la Bibliothèque d'authentification Active Directory (ADAL)**

- Nous vous recommandons d’effectuer la mise à jour vers MSAL, qui contient les dernières fonctionnalités et mises à jour de sécurité.
- Si vous utilisez des applications Microsoft, sachez que Microsoft est en train de migrer ses applications vers MSAL à l’échéance de fin du support, afin de s’assurer qu’elles pourront bénéficier des améliorations apportées en continu à la sécurité et aux fonctionnalités de MSAL.

1. [Lisez la FAQ sur la bibliothèque ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [En savoir plus sur la migration des applications selon la plateforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Si, après avoir lu le guide de la plateforme de votre application, vous avez d’autres questions, vous pouvez publier sur [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) avec la balise [azure-ad-adal-deprecation] ou ouvrir un problème dans le référentiel GitHub de la bibliothèque. Consultez la section [Langues et frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) de l'article de **présentation de MSAL** pour obtenir des liens vers le référentiel de chaque bibliothèque.
4. **Si vous avez besoin d'aide pour comprendre lesquelles de vos applications utilisent ADAL**, nous vous recommandons d'examiner le code source de toutes vos applications. Le cas échéant, contactez les fournisseurs indépendants de logiciels (ISV) ou les fournisseurs d'applications. L’équipe Support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre client.







