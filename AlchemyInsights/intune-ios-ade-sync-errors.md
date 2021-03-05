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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erreurs de synchronisation d’inscription automatique d’appareils Apple

« Nous avons détecté qu’un ou plusieurs jetons ADE/DEP seraient dans un état d’erreur. Tant que l’état d’erreur n’est pas résolu pour chaque jeton affecté, la fonctionnalité ADE ne fonctionne pas comme prévu. »

Cette erreur peut se manifester de plusieurs façons, notamment :

1. Les appareils peuvent ne pas être synchronisés entre ABM/ASM et Intune
2. Les affectations de profil d’inscription peuvent échouer
3. Les appareils risquent de ne pas réussir l’inscription ADE

Recherchez l’erreur de synchronisation signalée dans la console Intune sous Appareils > Inscrire des appareils **>'inscription Apple > jetons du programme d’inscription.**

L’une des causes les plus courantes d’une erreur de synchronisation est l’expiration du jeton actuel. Dans de nombreux cas, le renouvellement du jeton affecté résout le problème.

Si un ou plusieurs de vos jetons ont expiré, consultez la documentation suivante pour vous aider à les renouveler, le cas échéant :

[Renouveler un jeton d’inscription automatique d’appareil](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

En outre, vous pouvez consulter la documentation suivante pour voir les corrections potentielles pour d’autres erreurs à l’origine des échecs de synchronisation des jetons :

[Erreurs de synchronisation ABM/ASM pour les jetons d’inscription automatique des appareils iOS/iPadOS et macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Erreurs de synchronisation ABM/ASM pour les jetons d’inscription automatique des appareils iOS/iPadOS et macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
