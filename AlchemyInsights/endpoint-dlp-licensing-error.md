---
title: Erreur de licence DLP de point de terminaison
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
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090136"
---
# <a name="endpoint-dlp-licensing-error"></a>Erreur de licence DLP de point de terminaison

Lorsque vous essayez de configurer endpoint DLP, si vous recevez l’erreur suivante :

`Your organization is missing the licenses required to manage these devices`.

Assurez-vous que vous avez l’un des abonnements ou modules suivants :

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Conformité
- Microsoft 365 A5 Conformité
- Microsoft 365 E5, Protection des informations et gouvernance
- Microsoft 365 A5, Protection des informations et gouvernance

> [!NOTE]
> Cela ne fonctionne pas pour les combinaisons de licences telles que : Win E5 + O365 E5 + EMS E5. Vous devez avoir une licence M365 E5 pure pour configurer cette fonctionnalité.

Pour plus d’informations sur les licences DLP de point de [terminaison, voir Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
