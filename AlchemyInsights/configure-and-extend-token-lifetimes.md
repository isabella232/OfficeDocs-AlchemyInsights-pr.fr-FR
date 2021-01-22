---
title: Configurer et étendre la durée de vie des jetons
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911995"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="e22fd-102">Configurer et étendre la durée de vie des jetons</span><span class="sxs-lookup"><span data-stu-id="e22fd-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="e22fd-103">Vous pouvez spécifier la durée de vie d’un jeton d’accès, SAML, ou d’identification émis par la plateforme d’identité Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e22fd-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="e22fd-104">Vous pouvez définir les durées de vie des jetons pour toutes les applications de votre organisation, pour une application mutualisée (multi-organisation) ou pour un principal de service spécifique dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="e22fd-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="e22fd-105">Pour plus d’informations, lisez [Durée de vie des jetons configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="e22fd-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="e22fd-106">Pour consulter des exemples, [Exemples de la configuration de durées de vie des jetons](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="e22fd-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="e22fd-107">Pour découvrir comment configurer la durée de vie et la compatibilité d’un jeton dans Azure Active Directory B2C (Azure AD B2C), consultez[Configurer des jetons dans Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="e22fd-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="e22fd-108">L’article [Configurer le comportement des sessions dans Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) décrit les méthodes d’authentification unique (SSO) utilisées dans Azure AD B2C et vous aide à choisir la méthode d’authentification unique la plus appropriée lors de la configuration de votre stratégie.</span><span class="sxs-lookup"><span data-stu-id="e22fd-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="e22fd-109">**Durée de vie des jetons, durée de validité des jetons**</span><span class="sxs-lookup"><span data-stu-id="e22fd-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="e22fd-110">La durée de vie des jetons est 1 heure et la durée de vie des sessions est 24 heures.</span><span class="sxs-lookup"><span data-stu-id="e22fd-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="e22fd-111">Cela signifie que si aucune demande n’est faite au cours des 24 heures, vous devrez vous connecter à nouveau avant de demander un nouveau jeton.</span><span class="sxs-lookup"><span data-stu-id="e22fd-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="e22fd-112">Après le 30 mai 2020, aucun nouveau client ne pourra utiliser une stratégie de durée de vie des jetons configurable pour configurer des sessions et actualiser des jetons.</span><span class="sxs-lookup"><span data-stu-id="e22fd-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="e22fd-113">Le dépréciation se produira plusieurs mois après, ce qui signifie que nous dépasserons les sessions existantes pour actualiser les stratégies des jetons.</span><span class="sxs-lookup"><span data-stu-id="e22fd-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="e22fd-114">Vous pouvez toujours configurer les durées de vie des jetons d’accès après la dépréciation.</span><span class="sxs-lookup"><span data-stu-id="e22fd-114">You can still configure access token lifetimes after the deprecation.</span></span>






