---
title: Inventaire des appareils Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434607"
---
# <a name="intune-device-inventory"></a>Inventaire des appareils Intune

Le panneau Appareils fournit à l’administrateur des informations sur les appareils sous gestion dans Intune sur une base par appareil. Les informations présentées incluent les éléments suivants : matériel, applications détectées, état de conformité des appareils et état de configuration des appareils.

Les données d’inventaire du matériel et des applications découvertes sont collectées sur un cycle de 7 jours. Les applications et les éléments spécifiques du matériel signalé diffèrent selon le système d’exploitation de l’appareil et selon que l’appareil est possédé ou d’une entreprise.

Pour plus d’informations, consultez [Afficher les détails de l’appareil dans Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

Q : je ne reçois aucune liste d’inventaire complète des applications présentes sur les appareils Windows inscrits sur Intune. Pourquoi ?

R : pour le moment, seules les applications modernes sont répertoriées pour les PC Windows 10 identifiés en tant qu’appareils d’entreprise. Intune ne recueille pas d’informations sur les applications Win32 installées sur ces appareils.

Q : pourquoi les numéros de téléphone ne sont-ils pas collectés sur tous les appareils ?

R : les téléphones catégorisés en tant qu’appareils d’entreprise dans Intune ne sont pas identifiés avec leur numéro de téléphone complet lorsque, par exemple, vous exécutez un rapport sur l’inventaire des appareils mobiles. Les numéros de téléphone des appareils sont toujours partiellement masqués par des astérisques (****), et n'affichent que les quatre derniers chiffres.