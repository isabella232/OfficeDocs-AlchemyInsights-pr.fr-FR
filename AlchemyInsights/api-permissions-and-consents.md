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
# <a name="api-permissions-and-consent"></a><span data-ttu-id="6e407-102">Autorisations et consentement de l’API</span><span class="sxs-lookup"><span data-stu-id="6e407-102">API permissions and consent</span></span>

<span data-ttu-id="6e407-103">Les applications qui s’intègrent à la plateforme d’identités Microsoft suivent un modèle d’autorisation qui permet aux utilisateurs et aux administrateurs de contrôler la façon dont les données sont accessibles.</span><span class="sxs-lookup"><span data-stu-id="6e407-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="6e407-104">L’implémentation du modèle d’autorisation a été mise à jour sur le point de terminaison de la plateforme d’identités Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6e407-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="6e407-105">Cela modifie la façon dont une application doit interagir avec la plateforme d’identités Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6e407-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="6e407-106">[Les autorisations et le consentement](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dans le point de terminaison de la plateforme d’identités Microsoft couvrent les concepts de base de ce modèle d’autorisation, notamment les étendues, les autorisations et le consentement.</span><span class="sxs-lookup"><span data-stu-id="6e407-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="6e407-107">L’infrastructure de consentement [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilite le développement d’applications web et natives clientes multi-clients.</span><span class="sxs-lookup"><span data-stu-id="6e407-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="6e407-108">Ces applications autorisent la connectez-vous par des comptes d’utilisateur à partir d’un client Azure AD différent de celui dans lequel l’application est inscrite.</span><span class="sxs-lookup"><span data-stu-id="6e407-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="6e407-109">Ils peuvent également avoir besoin d’accéder aux API web telles que l’API Microsoft Graph (pour accéder à Azure AD, Intune et aux services dans Microsoft 365) et aux API d’autres services Microsoft, en plus de vos propres API web.</span><span class="sxs-lookup"><span data-stu-id="6e407-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

