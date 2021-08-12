---
title: Autorisations et consentement de l’API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932095"
---
# <a name="api-permissions-and-consent"></a>Autorisations et consentement de l’API

Les applications qui s’intègrent Plateforme d’identités Microsoft suivent un modèle d’autorisation qui permet aux utilisateurs et aux administrateurs de contrôler la façon dont les données sont accessibles. L’implémentation du modèle d’autorisation a été mise à jour Plateforme d’identités Microsoft point de terminaison. Cela modifie la façon dont une application doit interagir avec le Plateforme d’identités Microsoft. [Les autorisations et le](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) consentement dans le point de terminaison Plateforme d’identités Microsoft traitent des concepts de base de ce modèle d’autorisation, notamment les étendues, les autorisations et le consentement.

[L Azure Active Directory de consentement (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilite le développement d’applications clientes web et natives multi-clients. Ces applications autorisent la connectez-vous par des comptes d’utilisateur à partir d’un client Azure AD différent de celui où l’application est inscrite. Ils peuvent également avoir besoin d’accéder aux API web telles que l’API Microsoft Graph (pour accéder à Azure AD, Intune et aux services dans Microsoft 365) et autres API de services Microsoft, en plus de vos propres API web.

