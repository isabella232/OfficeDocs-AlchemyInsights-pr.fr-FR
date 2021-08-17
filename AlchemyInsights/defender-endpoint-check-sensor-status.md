---
title: État des points de terminaison Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: cefebe63e45caab176ba84a35280378ace7e6b3115c48694ed043a39b4d93c1e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890052"
---
# <a name="defender-endpoint-check-sensor-status"></a>État des points de terminaison Defender

La vignette **Appareils avec problèmes de détection.** est située dans le tableau de bord opérations de sécurité. Cette vignette fournit des informations sur la capacité de chaque appareil à fournir des données de détection à communiquer avec le service Defender pour point de terminaison. Elle indique le nombre d’appareils qui nécessitent une attention particulière et vous aide à identifier les appareils problématiques et à prendre des mesures pour les corriger.

Deux indicateurs d’état sur la vignette fournissent des informations sur le nombre d’appareils qui ne rapportent pas correctement au service :

- **Mal configurés** Appareils qui peuvent signaler partiellement des données de détection au service Defender pour point de terminaison et qui peuvent présenter des erreurs de configuration devant être corrigées.
- **Inactifs** Appareils qui ont cessé de rendre compte au service Defender pour le point de terminaison pendant plus de sept jours au cours du mois précédent.

En cliquant sur l'un des groupes, vous accédez à la liste Appareils, filtrée en fonction de vos choix. Dans la liste Appareils, vous pouvez filtrer la liste d’état d’intégrité selon l’état suivant :

- **Actifs** Appareils signalés activement au service Defender pour point de terminaison.
- **Mal configurés** Appareils qui peuvent signaler partiellement des données de détection au service Defender pour points de terminaison, mais présentent des erreurs de configuration devant être corrigées. Les appareils mal configurés peuvent avoir l’un ou l’autre des problèmes suivants :

    - Aucune donnée de détection : les appareils ont arrêté d’envoyer des données de détection. Des alertes limitées peuvent être déclenchées à partir de l’appareil.
    - Communications altérées : la capacité de communiquer avec l’appareil est altérée. L’envoi de fichiers pour une analyse approfondie, le blocage de fichiers, l’isolation de l’appareil du réseau et d’autres actions qui nécessitent une communication avec l’appareil peuvent ne pas fonctionner.
- **Inactifs** Appareils qui ont cessé de rendre compte au service Defender pour le point de terminaison.

Vous pouvez télécharger la liste entière au format CSV à l'aide de la fonctionnalité Exporter.

Pour plus d’informations, consultez [Vérifier l'état d'intégrité de détection dans Microsoft Defender pour point de terminaison](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status).

Pour plus d’informations sur la cause de l’inactivité ou de la configuration d’un appareil, consultez [Corriger les détecteurs malsains dans Microsoft Defender pour point de terminaison](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
