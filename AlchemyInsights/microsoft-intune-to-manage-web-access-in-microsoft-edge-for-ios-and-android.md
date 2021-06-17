---
title: Utiliser Microsoft Intune pour gérer l’accès web dans Microsoft Edge pour iOS et Android
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
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989666"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="70af5-102">Utiliser Microsoft Intune pour gérer l’accès web dans Microsoft Edge pour iOS et Android</span><span class="sxs-lookup"><span data-stu-id="70af5-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="70af5-103">Microsoft Edge pour iOS et Android permet à un utilisateur de parcourir le web à partir de plusieurs profils totalement distincts.</span><span class="sxs-lookup"><span data-stu-id="70af5-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="70af5-104">Les fonctionnalités de protection les plus étendues pour Microsoft 365 données sont disponibles lorsque vous vous abonnez à la suite Enterprise Mobility + Security, qui inclut des fonctionnalités Microsoft Intune et Azure Active Directory Premium, telles que l’accès conditionnel.</span><span class="sxs-lookup"><span data-stu-id="70af5-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="70af5-105">Au minimum, vous souhaiterez déployer une stratégie d’accès conditionnel qui (1) permet aux utilisateurs de se connecter à partir d’appareils mobiles à Microsoft Edge pour iOS et Android et qui (2) implémente une stratégie de protection des applications Microsoft Intune qui fournit une expérience de navigation protégée.</span><span class="sxs-lookup"><span data-stu-id="70af5-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="70af5-106">Pour comprendre comment utiliser l’accès conditionnel et les stratégies, voir :</span><span class="sxs-lookup"><span data-stu-id="70af5-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="70af5-107">Appliquer des Azure Active Directory d’accès conditionnel aux données</span><span class="sxs-lookup"><span data-stu-id="70af5-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="70af5-108">Créer des stratégies Microsoft Intune protection des applications</span><span class="sxs-lookup"><span data-stu-id="70af5-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="70af5-109">Utiliser l' sign-on unique Azure Active Directory applications web connectées dans des navigateurs protégés par la stratégie</span><span class="sxs-lookup"><span data-stu-id="70af5-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="70af5-110">Utiliser la configuration de l’application pour gérer l’expérience de navigation</span><span class="sxs-lookup"><span data-stu-id="70af5-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="70af5-111">Autoriser l’utilisation des comptes scolaires et de travail uniquement</span><span class="sxs-lookup"><span data-stu-id="70af5-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="70af5-112">Déployer des stratégies générales de configuration d’application</span><span class="sxs-lookup"><span data-stu-id="70af5-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="70af5-113">Déployer des stratégies de configuration d’application pour la protection des données</span><span class="sxs-lookup"><span data-stu-id="70af5-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="70af5-114">Utiliser Microsoft Endpoint Manager pour déployer des stratégies de configuration d’application</span><span class="sxs-lookup"><span data-stu-id="70af5-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="70af5-115">Pour découvrir comment accéder aux journaux des applications gérées, voir Utiliser Microsoft Edge pour iOS et Android pour accéder aux journaux des applications [gérées.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="70af5-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
