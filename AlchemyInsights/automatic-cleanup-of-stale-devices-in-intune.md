---
title: Nettoyage automatique des appareils obsolètes dans Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997070"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Nettoyage automatique des appareils obsolètes dans Intune

Intune permet à l’administrateur de configurer un intervalle de temps compris entre 90 et 270 jours, après quoi les appareils obsolètes sont supprimés du service. Ce paramètre s’applique à l’échelle de l’organisation et une fois activés immédiatement. Les appareils non archivés dans le serveur Intune pendant une période supérieure au paramètre sont supprimés définitivement.

**Remarque** seuls les objets appareil de la gestion des appareils mobiles sont éligibles pour cette action de nettoyage. Seuls les objets de l'appareil EAS sont exclus.

Pour plus d’informations sur la suppression d’un appareil sur la base du paramètre de nettoyage de l’appareil et de son « état », procédez comme suit :

Paramètre : **supprimer les appareils après la dernière date d’archivage : Oui (valeur (N) dans jours spécifiés)**

- En fonction de la valeur (N) configurée dans le paramètre, le service Intune supprime l’appareil dans les jours spécifiés après son dernier enregistrement réussi.

Paramètre : **supprimer les appareils après la dernière date d’archivage : non**

- 180 jours après l'expiration et le non-renouvellement du certificat de l'appareil, celui-ci est supprimé.

**Remarque** dans les deux cas, l’appareil doit être correctement inscrit dans Intune. L’inscription a lieu pendant la première intégration de l’appareil avec le service Intune.

Si un appareil se met en relation avec Intune, mais qu’il n’a pas été inscrits dans Intune, l’appareil est supprimé 270 jours après l’inscription. (90 jours pour marquer l’appareil comme révoqué, puis un autre 180 jours pour supprimer l’enregistrement.)

Il n’existe actuellement aucun mécanisme dans la console Intune pour définir la date d’expiration de la certification des appareils pour un appareil donné.