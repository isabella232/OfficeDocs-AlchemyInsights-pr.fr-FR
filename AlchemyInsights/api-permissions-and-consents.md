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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951893"
---
# <a name="api-permissions-and-consent"></a>Autorisations et consentement de l’API

Les applications qui s’intègrent à la plateforme d’identités Microsoft suivent un modèle d’autorisation qui permet aux utilisateurs et aux administrateurs de contrôler la façon dont les données sont accessibles. L’implémentation du modèle d’autorisation a été mise à jour sur le point de terminaison de la plateforme d’identités Microsoft. Cela modifie la façon dont une application doit interagir avec la plateforme d’identités Microsoft. [Les autorisations et le consentement](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dans le point de terminaison de la plateforme d’identités Microsoft couvrent les concepts de base de ce modèle d’autorisation, notamment les étendues, les autorisations et le consentement.

L’infrastructure de consentement [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilite le développement d’applications web et natives clientes multi-clients. Ces applications autorisent la connectez-vous par des comptes d’utilisateur à partir d’un client Azure AD différent de celui dans lequel l’application est inscrite. Ils peuvent également avoir besoin d’accéder aux API web telles que l’API Microsoft Graph (pour accéder à Azure AD, Intune et aux services dans Microsoft 365) et aux API d’autres services Microsoft, en plus de vos propres API web.

