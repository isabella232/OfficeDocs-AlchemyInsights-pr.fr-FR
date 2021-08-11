---
title: Configuration du proxy d’application
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951563"
---
# <a name="app-proxy-configuration"></a>Configuration du proxy d’application

1. Pour comprendre comment configurer une application proxy d’application dans Azure AD pour exposer vos applications sur site au cloud, voir Comment configurer une [application proxy d’application.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. L’authentification unique (SSO) permet à vos utilisateurs d’accéder à une application sans s’authentifier plusieurs fois. Il permet à l’authentification unique de se produire dans le cloud, par rapport à Azure Active Directory, et permet au service ou au connecteur d’usurper l’identité de l’utilisateur pour relever d’autres défis d’authentification de l’application. Pour plus d’informations, [voir Comment configurer l' sign-on unique sur une application proxy d’application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Utilisez [cet article pour](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) résoudre les problèmes courants que rencontrent les personnes lors de la création d’une application proxy d’application.
4. Si vous avez un problème lors de la configuration de l’authentification back-end sur votre application, vous devrez peut-être résoudre les configurations de délégation [Kerberos contraintes](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) pour le proxy d’application ou suivre des instructions sur la configuration de l’application avec [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) pour résoudre votre problème.
