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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erreurs de synchronisation d’inscriptions automatiques d’appareil Apple

«Nous avons détecté que vous avez un ou plusieurs jetons ADE/DEP en état d’erreur. Tant que l’état de l’erreur n’est pas résolu pour chaque jeton concerné, la fonctionnalité ADE ne fonctionnera pas pour le même «.

Cette erreur peut se manifester de plusieurs façons, notamment :

1. Les appareils ne peuvent pas être synchronisés à partir de ABM/ASM vers Intune
2. Les affectations de profil d’inscriptions peuvent échouer
3. Les appareils ne peuvent pas terminer l’enregistrement ADE correctement

Recherchez l’erreur de synchronisation signalée dans la console Intune sous **périphériques > inscrire des appareils > jetons d’inscription > Apple** , puis examinez la documentation suivante pour voir toute correction potentielle :

[Erreurs de synchronisation ABM/ASM pour les jetons d’inscriptions automatisées de l’appareil iOS/iPados et macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
