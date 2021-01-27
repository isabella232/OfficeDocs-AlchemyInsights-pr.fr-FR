---
title: Problèmes lors du développement d’applications
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950734"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="0fa2b-102">Problèmes lors du développement d’applications</span><span class="sxs-lookup"><span data-stu-id="0fa2b-102">Issues developing applications</span></span>

<span data-ttu-id="0fa2b-103">Pour résoudre les problèmes les plus courants lors de la création d’applications Azure Active Directory (AD), veuillez consulter les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="0fa2b-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- <span data-ttu-id="0fa2b-104">[J’ai des problèmes de connexion à une ou plusieurs applications à l’aide du navigateur Chrome uniquement](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="0fa2b-104">[I am seeing trouble signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span></span> 
- [<span data-ttu-id="0fa2b-105">Je ne sais pas comment modifier les valeurs par défaut de la durée de vie des jetons pour mon application</span><span class="sxs-lookup"><span data-stu-id="0fa2b-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="0fa2b-106">Je suis perplexe quant au fonctionnement du consentement concernant les applications</span><span class="sxs-lookup"><span data-stu-id="0fa2b-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="0fa2b-107">Je ne sais pas comment accorder des autorisations à mon application</span><span class="sxs-lookup"><span data-stu-id="0fa2b-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="0fa2b-108">Je ne comprends pas la différence entre les autorisations déléguées et les autorisations d’application</span><span class="sxs-lookup"><span data-stu-id="0fa2b-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="0fa2b-109">\***Fin de la prise en charge de la Bibliothèque d’authentification Azure Active Directory (ADAL) et de l’API Azure AD Graph (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="0fa2b-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="0fa2b-110">À compter du 30 juin 2020, nous n’ajouterons plus de nouvelles fonctionnalités à la Bibliothèque d’authentification Azure Active Directory (ADAL) et à l’API Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="0fa2b-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="0fa2b-111">Nous continuerons à fournir une assistance technique et des mises à jour de sécurité, mais nous ne fournirons plus de mises à jour de fonctionnalités.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="0fa2b-112">À compter du 30 juin 2022, nous allons mettre fin à la prise en charge de la bibliothèque ADAL et d’AAD Graph ; nous ne fournirons plus de support technique, ni de mises à jour de sécurité.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="0fa2b-113">Par conséquent, les implications sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="0fa2b-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="0fa2b-114">Les applications qui utilisent ADAL sur les versions existantes du système d’exploitation continueront de fonctionner après cette période, mais ne bénéficieront pas d’un quelconque support technique, ni de mises à jour de sécurité.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="0fa2b-115">Les applications utilisant Azure AD Graph après cette période risquent de ne plus recevoir de réponses du point de terminaison AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="0fa2b-116">_ *Migration de la bibliothèque ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="0fa2b-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="0fa2b-117">Si vous utilisez des applications Microsoft, nous vous recommandons d’effectuer la mise à jour vers la bibliothèque d’authentification Microsoft (MSAL), qui contient les dernières fonctionnalités et mises à jour de sécurité.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="0fa2b-118">Nous émettons cette recommandation dans le contexte suivant : Microsoft a lancé le processus de migration de ses applications vers la bibliothèque MSAL avant la fin du support technique.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="0fa2b-119">La migration, par Microsoft, de ses applications vers la bibliothèque MSAL garantit que les applications bénéficient des améliorations constantes apportées par cette bibliothèque en matière de sécurité et de fonctionnalités.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="0fa2b-120">Lisez la FAQ sur la bibliothèque ADAL</span><span class="sxs-lookup"><span data-stu-id="0fa2b-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="0fa2b-121">En savoir plus sur la migration des applications selon la plateforme</span><span class="sxs-lookup"><span data-stu-id="0fa2b-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="0fa2b-122">Si vous avez besoin d’aide pour comprendre quelles sont vos applications qui utilisent ADAL, nous vous recommandons d’évaluer le code source de toutes vos applications et, le cas échéant, de faire appel à des éditeurs de logiciels indépendants ou à des fournisseurs d’applications.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="0fa2b-123">Le support Microsoft peut également vous fournir une liste de toutes les applications ADAL non Microsoft de votre client.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="0fa2b-124">**Migration des applications AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="0fa2b-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="0fa2b-125">Veuillez suivre nos recommandations pour migrer les applications AAD Graph vers Microsoft Graph :</span><span class="sxs-lookup"><span data-stu-id="0fa2b-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="0fa2b-126">[Notre liste de contrôle de la migration fournit un point de mise en route](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="0fa2b-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="0fa2b-127">Votre portail d’inscription d’applications Azure indique les applications qui utilisent AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="0fa2b-128">Nous vous recommandons d’évaluer le code source de toutes vos applications et, le cas échéant, de faire appel à des éditeurs de logiciels indépendants ou à des fournisseurs d’applications.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="0fa2b-129">Le support Microsoft peut également vous fournir des informations sur l’utilisation d’AAD Graph dans votre client.</span><span class="sxs-lookup"><span data-stu-id="0fa2b-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







