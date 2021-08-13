---
title: Résoudre les problèmes de consentement de l’utilisateur
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007896"
---
# <a name="troubleshoot-user-consent"></a>Résoudre les problèmes de consentement de l’utilisateur

1. Vous pouvez configurer la façon dont les utilisateurs finaux consentent aux applications via le portail Azure ou PowerShell. Pour plus [d’informations, voir paramètres](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) de consentement utilisateur.
1. Un administrateur peut également utiliser [l’API microsoft Graph pour](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) accorder le consentement aux autorisations déléguées au nom d’un seul utilisateur. Pour plus d’informations, [voir Obtenir l’accès au nom d’un utilisateur.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Erreurs de consentement de](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)l’utilisateur : cet article traite des erreurs qui peuvent se produire pendant le processus de consentement à une application. Si vous dépannagez des invites de consentement inattendues qui ne contiennent aucun message d’erreur, consultez Scénarios d’authentification [pour Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).