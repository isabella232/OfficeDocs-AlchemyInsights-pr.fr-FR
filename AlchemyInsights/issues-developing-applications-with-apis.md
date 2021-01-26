---
title: Problèmes de développement d’applications avec des API
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
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951899"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="759ec-102">Problèmes de développement d’applications avec des API</span><span class="sxs-lookup"><span data-stu-id="759ec-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="759ec-103">Pour commencer à utiliser l’API Azure Active Directory Graph, consultez le guide de démarrage rapide de [l’API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ou consultez la documentation de référence interactive de l’API Azure [AD Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="759ec-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="759ec-104">**Fin de la prise en charge d’Azure Active Directory Authentication Library (ADAL) et de l’API Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="759ec-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="759ec-105">**À compter du 30 juin 2020,** nous n’ajouterons plus de nouvelles fonctionnalités à ADAL et Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="759ec-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="759ec-106">Nous continuerons à fournir un support technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.</span><span class="sxs-lookup"><span data-stu-id="759ec-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="759ec-107">À compter **du 30 juin 2022,** nous arrêterons la prise en charge d’ADAL et d’Azure AD Graph et ne fournirons plus de support technique ni de mises à jour de sécurité.</span><span class="sxs-lookup"><span data-stu-id="759ec-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="759ec-108">Les applications utilisant ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais n’auront pas de support technique ou de mises à jour de sécurité.</span><span class="sxs-lookup"><span data-stu-id="759ec-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="759ec-109">Les applications utilisant Azure AD Graph après cette période peuvent ne plus recevoir de réponses du point de terminaison Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="759ec-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="759ec-110">**ADAL Migration**</span><span class="sxs-lookup"><span data-stu-id="759ec-110">**ADAL Migration**</span></span>

<span data-ttu-id="759ec-111">Nous vous recommandons de mettre à jour la bibliothèque d’authentification [Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)qui dispose des dernières fonctionnalités et mises à jour de sécurité.</span><span class="sxs-lookup"><span data-stu-id="759ec-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="759ec-112">Si vous utilisez des applications Microsoft, sachez que Microsoft est en train de migrer ses applications vers MSAL à l’échéance de fin du support, en veillant à ce qu’elles bénéficient des améliorations constantes de la sécurité et des fonctionnalités de MSAL.</span><span class="sxs-lookup"><span data-stu-id="759ec-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="759ec-113">[Lisez le FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="759ec-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="759ec-114">[Découvrez comment migrer des applications par plateforme.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="759ec-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="759ec-115">Si vous avez besoin d’aide pour savoir quelles applications utilisent ADAL, nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, d’atteindre les fournisseurs de logiciels indépendants ou les fournisseurs d’applications.</span><span class="sxs-lookup"><span data-stu-id="759ec-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="759ec-116">Le support Microsoft peut également vous fournir une liste de toutes les applications non-Microsoft ADAL de votre client.</span><span class="sxs-lookup"><span data-stu-id="759ec-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="759ec-117">**AAD Graph Migration**</span><span class="sxs-lookup"><span data-stu-id="759ec-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="759ec-118">Pour les applications qui utilisent Azure AD Graph, suivez nos instructions pour migrer des applications [Azure AD Graph vers Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="759ec-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="759ec-119">[Notre liste de contrôle de migration fournit un point de départ.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="759ec-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="759ec-120">Votre portail d’inscription d’application Azure indique les applications qui utilisent AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="759ec-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="759ec-121">Nous vous recommandons de passer en revue l’ensemble du code source de vos applications et, le cas échéant, de joindre des fournisseurs de logiciels indépendants ou des fournisseurs d’applications.</span><span class="sxs-lookup"><span data-stu-id="759ec-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="759ec-122">Le support Microsoft peut également vous fournir une liste de toutes les utilisations d’AAD Graph dans votre client.</span><span class="sxs-lookup"><span data-stu-id="759ec-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="759ec-123">Pour que votre application puisse accéder aux données dans Microsoft Graph, l’utilisateur ou l’administrateur doivent lui accorder les autorisations appropriées via un processus de consentement.</span><span class="sxs-lookup"><span data-stu-id="759ec-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="759ec-124">La [référence des autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) répertorie les autorisations associées à chaque ensemble majeur d’API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="759ec-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="759ec-125">Elle fournit également des instructions sur l’utilisation des autorisations.</span><span class="sxs-lookup"><span data-stu-id="759ec-125">It also provides guidance about how to use the permissions.</span></span>
