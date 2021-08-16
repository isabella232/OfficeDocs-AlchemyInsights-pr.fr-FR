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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028074"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problèmes avec une ressource ou un principal de service

1. Si vous ne faites que commencer, les objets application et principal de service dans [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) décrivent l’inscription de l’application, les objets d’application et les principaux de service dans Azure Active Directory : ce qu’ils sont, comment ils sont utilisés et comment ils sont liés les uns aux autres. Un exemple de scénario à plusieurs clients est également présenté pour illustrer la relation entre l’objet d’application d’une application et les objets principaux de service correspondants.
2. Vous pouvez en savoir plus sur la relation entre les applications et les principaux de service en lisant les applications et les objets principaux de [service dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Avec [l’API de principal](https://docs.microsoft.com/graph/api/resources/serviceprincipal)de service, vous pouvez gérer par programme des instances d’applications et contrôler ce qu’une application peut faire au sein de votre client.
5. [Le type de ressource servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) répertorie toutes les propriétés et méthodes pour le type de ressource servicePrincipal.
6. [Les différences](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) de type de ressource entre Azure AD Graph et Microsoft Graph soulignent les différences entre azure AD Graph et les ressources Graph Microsoft. Il affiche les ressources qui ont des noms différents ou qui ne sont pas disponibles ; Il met également en évidence les ressources disponibles dans la version bêta de Microsoft Graph mais pas dans la version v1.0.

**Problèmes avec les utilisateurs invités**

- Démarrage rapide : ajouter des utilisateurs invités à votre annuaire dans le portail [Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vous montre comment ajouter un nouvel utilisateur invité à votre annuaire Azure AD via le portail Azure, envoyer une invitation et voir à quoi ressemble le processus d’échange d’invitation de l’utilisateur invité.
- [Didacticiel : Créer des flux d’utilisateurs Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) vous montre comment créer des flux d’utilisateurs recommandés à l’aide du portail Azure. Si vous recherchez des informations sur la configuration d’un flux ROPC (Resource Owner Password Credentials) dans votre application, voir Configurer le flux d’informations d’identification du mot de passe du propriétaire de la ressource dans Azure AD B2C.
