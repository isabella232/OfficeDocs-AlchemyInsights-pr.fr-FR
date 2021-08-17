---
title: Problèmes de suppression d’un appareil désintôt ou désaffecté de l’inventaire des appareils
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076650"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problèmes de suppression d’un appareil désintôt ou désaffecté de l’inventaire des appareils

Microsoft Defender pour le point de terminaison n’autorise pas actuellement la suppression manuelle de l’enregistrement d’appareil d’un appareil désintôt ou désaffecté de l’inventaire des appareils.

À des fins de sécurité, l’appareil reste dans le portail en tant qu’enregistrement historique pendant 180 jours au plus. Toutefois, les données de l’appareil sont purgées en fonction de votre période de rétention configurée.

**Remarque :** Un appareil désint res ou désaffecté passe automatiquement à **l’état Inactif** au bout de sept jours. En outre, les appareils non actifs au cours des 30 derniers jours ne sont pas pris en compte dans les données qui reflètent le score d’exposition de votre organisation Gestion des menaces et des vulnérabilités ou le score de sécurité Microsoft pour les appareils.
 
Si vous ne souhaitez toujours pas voir certains appareils en affichage Inventaire des appareils, essayez de placer une balise d’appareil pour filtrer l’appareil désaffecté de l’affichage Inventaire des appareils.

Pour plus d’informations, voir :

[Hors-carte des appareils à partir du service Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Score d’exposition en Gestion des menaces et des vulnérabilités](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Corriger les capteurs défectueux dans Microsoft Defender pour le point de terminaison](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Utilisation efficace du balisage (partie 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Utilisation efficace du balisage (partie 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Utilisation efficace du balisage (partie 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




