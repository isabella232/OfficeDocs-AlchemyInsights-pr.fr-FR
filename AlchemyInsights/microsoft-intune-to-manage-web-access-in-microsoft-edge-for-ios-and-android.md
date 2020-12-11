---
title: Utiliser Microsoft Intune pour gérer l’accès Web dans Microsoft Edge pour iOS et Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617245"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="1407c-102">Utiliser Microsoft Intune pour gérer l’accès Web dans Microsoft Edge pour iOS et Android</span><span class="sxs-lookup"><span data-stu-id="1407c-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="1407c-103">Microsoft Edge pour iOS et Android permet à un utilisateur de naviguer sur le Web à partir de plusieurs profils entièrement distincts.</span><span class="sxs-lookup"><span data-stu-id="1407c-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="1407c-104">Les fonctionnalités de protection les plus étendues pour les données Microsoft 365 deviennent disponibles lorsque vous vous abonnez à la suite Enterprise Mobility + Security, qui inclut les fonctionnalités Microsoft Intune et Azure Active Directory Premium, telles que l’accès conditionnel.</span><span class="sxs-lookup"><span data-stu-id="1407c-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="1407c-105">Au minimum, vous souhaiterez déployer une stratégie d’accès conditionnel qui (1) permet aux utilisateurs de se connecter depuis des appareils mobiles à Microsoft Edge pour iOS et Android et que (2) implémente une stratégie de protection d’application Microsoft Intune qui offre une expérience de navigation protégée.</span><span class="sxs-lookup"><span data-stu-id="1407c-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="1407c-106">Pour comprendre comment utiliser l’accès conditionnel et les stratégies, voir :</span><span class="sxs-lookup"><span data-stu-id="1407c-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="1407c-107">Appliquer des stratégies d’accès conditionnel Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1407c-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="1407c-108">Créer des stratégies de protection d’application Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1407c-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="1407c-109">Utiliser l’authentification unique pour les applications Web connectées à Azure Active Directory dans les navigateurs protégés par des stratégies</span><span class="sxs-lookup"><span data-stu-id="1407c-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="1407c-110">Utiliser la configuration de l’application pour gérer l’expérience de navigation</span><span class="sxs-lookup"><span data-stu-id="1407c-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="1407c-111">Autoriser l’utilisation de comptes professionnels et scolaires uniquement</span><span class="sxs-lookup"><span data-stu-id="1407c-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="1407c-112">Déployer des stratégies de configuration d’application générales</span><span class="sxs-lookup"><span data-stu-id="1407c-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="1407c-113">Déployer des stratégies de configuration d’application pour la protection des données</span><span class="sxs-lookup"><span data-stu-id="1407c-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="1407c-114">Utiliser le gestionnaire de points de terminaison Microsoft pour déployer des stratégies de configuration d’application</span><span class="sxs-lookup"><span data-stu-id="1407c-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="1407c-115">Pour savoir comment accéder aux journaux d’applications gérées, consultez la rubrique [utilisation de Microsoft Edge pour iOS et Android pour accéder aux journaux d’applications gérées](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="1407c-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
