---
title: Problèmes avec une ressource ou un principal de service
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716125"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problèmes avec une ressource ou un principal de service

1. Si vous ne faites que commencer, les objets application et principal de service dans [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) décrivent l’inscription des applications, les objets d’application et les principaux de service dans Azure Active Directory : ce qu’ils sont, comment ils sont utilisés et comment ils sont liés les uns aux autres. Un exemple de scénario à plusieurs clients est également présenté pour illustrer la relation entre l’objet d’application d’une application et les objets principaux de service correspondants.
2. Vous pouvez en savoir plus sur la relation entre les applications et les principaux de service en lisant des applications et des objets principaux de [service dans Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. La procédure : utiliser le portail pour créer une [application Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) et un principal de service qui peuvent accéder aux ressources vous montre comment créer une application Azure Active Directory (Azure AD) et un principal de service qui peuvent être utilisés avec le contrôle d’accès basé sur un rôle.
4. Avec [l’API de principal](https://docs.microsoft.com/graph/api/resources/serviceprincipal)de service, vous pouvez gérer par programme des instances d’applications et contrôler ce qu’une application peut faire au sein de votre client.
5. [Le type de ressource servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) répertorie toutes les propriétés et méthodes pour le type de ressource servicePrincipal.
6. [Les différences de type](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) de ressource entre Azure AD Graph et Microsoft Graph soulignent les différences entre les ressources Azure AD Graph et Microsoft Graph. Il affiche les ressources qui ont des noms différents ou qui ne sont pas disponibles ; Il met également en évidence les ressources disponibles dans la version bêta de Microsoft Graph, mais pas dans la version v1.0.

**Problèmes avec les utilisateurs invités**

- Démarrage rapide : ajouter des utilisateurs invités à votre annuaire dans le portail [Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vous montre comment ajouter un nouvel utilisateur invité à votre annuaire Azure AD via le portail Azure, envoyer une invitation et voir à quoi ressemble le processus d’échange d’invitation de l’utilisateur invité.
- [Didacticiel : créer des](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) flux d’utilisateurs dans Azure Active Directory B2C vous montre comment créer des flux d’utilisateurs recommandés à l’aide du portail Azure. Si vous recherchez des informations sur la configuration d’un flux ROPC (Resource Owner Password Credentials) dans votre application, voir Configurer le flux d’informations d’identification du mot de passe du propriétaire de la ressource dans Azure AD B2C.
