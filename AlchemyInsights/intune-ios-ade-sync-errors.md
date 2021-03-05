---
title: Erreurs de synchronisation d’inscription automatique d’appareils Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448920"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="1eaad-102">Erreurs de synchronisation d’inscription automatique d’appareils Apple</span><span class="sxs-lookup"><span data-stu-id="1eaad-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="1eaad-103">« Nous avons détecté qu’un ou plusieurs jetons ADE/DEP seraient dans un état d’erreur.</span><span class="sxs-lookup"><span data-stu-id="1eaad-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="1eaad-104">Tant que l’état d’erreur n’est pas résolu pour chaque jeton affecté, la fonctionnalité ADE ne fonctionne pas comme prévu. »</span><span class="sxs-lookup"><span data-stu-id="1eaad-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="1eaad-105">Cette erreur peut se manifester de plusieurs façons, notamment :</span><span class="sxs-lookup"><span data-stu-id="1eaad-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="1eaad-106">Les appareils peuvent ne pas être synchronisés entre ABM/ASM et Intune</span><span class="sxs-lookup"><span data-stu-id="1eaad-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="1eaad-107">Les affectations de profil d’inscription peuvent échouer</span><span class="sxs-lookup"><span data-stu-id="1eaad-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="1eaad-108">Les appareils risquent de ne pas réussir l’inscription ADE</span><span class="sxs-lookup"><span data-stu-id="1eaad-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="1eaad-109">Recherchez l’erreur de synchronisation signalée dans la console Intune sous Appareils > Inscrire des appareils **>'inscription Apple > jetons du programme d’inscription.**</span><span class="sxs-lookup"><span data-stu-id="1eaad-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="1eaad-110">L’une des causes les plus courantes d’une erreur de synchronisation est l’expiration du jeton actuel.</span><span class="sxs-lookup"><span data-stu-id="1eaad-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="1eaad-111">Dans de nombreux cas, le renouvellement du jeton affecté résout le problème.</span><span class="sxs-lookup"><span data-stu-id="1eaad-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="1eaad-112">Si un ou plusieurs de vos jetons ont expiré, consultez la documentation suivante pour vous aider à les renouveler, le cas échéant :</span><span class="sxs-lookup"><span data-stu-id="1eaad-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="1eaad-113">Renouveler un jeton d’inscription automatique d’appareil</span><span class="sxs-lookup"><span data-stu-id="1eaad-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="1eaad-114">En outre, vous pouvez consulter la documentation suivante pour voir les corrections potentielles pour d’autres erreurs à l’origine des échecs de synchronisation des jetons :</span><span class="sxs-lookup"><span data-stu-id="1eaad-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="1eaad-115">Erreurs de synchronisation ABM/ASM pour les jetons d’inscription automatique des appareils iOS/iPadOS et macOS</span><span class="sxs-lookup"><span data-stu-id="1eaad-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="1eaad-116">Erreurs de synchronisation ABM/ASM pour les jetons d’inscription automatique des appareils iOS/iPadOS et macOS</span><span class="sxs-lookup"><span data-stu-id="1eaad-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
