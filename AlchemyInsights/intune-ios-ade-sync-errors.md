---
title: Erreurs de synchronisation d’inscriptions automatiques d’appareil Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707869"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="b5e82-102">Erreurs de synchronisation d’inscriptions automatiques d’appareil Apple</span><span class="sxs-lookup"><span data-stu-id="b5e82-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="b5e82-103">«Nous avons détecté que vous avez un ou plusieurs jetons ADE/DEP en état d’erreur.</span><span class="sxs-lookup"><span data-stu-id="b5e82-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="b5e82-104">Tant que l’état de l’erreur n’est pas résolu pour chaque jeton concerné, la fonctionnalité ADE ne fonctionnera pas pour le même «.</span><span class="sxs-lookup"><span data-stu-id="b5e82-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="b5e82-105">Cette erreur peut se manifester de plusieurs façons, notamment :</span><span class="sxs-lookup"><span data-stu-id="b5e82-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="b5e82-106">Les appareils ne peuvent pas être synchronisés à partir de ABM/ASM vers Intune</span><span class="sxs-lookup"><span data-stu-id="b5e82-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="b5e82-107">Les affectations de profil d’inscriptions peuvent échouer</span><span class="sxs-lookup"><span data-stu-id="b5e82-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="b5e82-108">Les appareils ne peuvent pas terminer l’enregistrement ADE correctement</span><span class="sxs-lookup"><span data-stu-id="b5e82-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="b5e82-109">Recherchez l’erreur de synchronisation signalée dans la console Intune sous **périphériques > inscrire des appareils > jetons d’inscription > Apple** , puis examinez la documentation suivante pour voir toute correction potentielle :</span><span class="sxs-lookup"><span data-stu-id="b5e82-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="b5e82-110">Erreurs de synchronisation ABM/ASM pour les jetons d’inscriptions automatisées de l’appareil iOS/iPados et macOS</span><span class="sxs-lookup"><span data-stu-id="b5e82-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
