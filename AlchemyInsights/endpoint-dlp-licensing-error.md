---
title: Erreur de licence DLP pour le point de terminaison
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477670"
---
# <a name="endpoint-dlp-licensing-error"></a>Erreur de licence DLP pour le point de terminaison

Lorsque vous essayez de configurer le point de terminaison DLP, si vous recevez l’erreur suivante :

`Your organization is missing the licenses required to manage these devices`.

Vérifiez que vous disposez de l’un des abonnements ou des modules complémentaires suivants :

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Conformité
- Microsoft 365 A5 Conformité
- Microsoft 365 E5, Protection des informations et gouvernance
- Microsoft 365 A5, Protection des informations et gouvernance

> [!NOTE]
> Cela ne fonctionne pas pour les combinaisons de licences comme : Win E5 + O365 E5 + EMS E5. Vous devez disposer d’une licence pure M365 E5 pour configurer cette fonctionnalité.

Pour plus d’informations sur la gestion des licences DLP, consultez la rubrique gestion des [licences de point de terminaison DLP.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
