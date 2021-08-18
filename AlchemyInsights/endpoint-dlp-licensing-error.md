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
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322129"
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

**Remarque**: cela ne fonctionne pas pour les combinaisons de licences telles que : Win E5 + O365 E5 + EMS E5. Vous devez avoir une licence M365 E5 pure pour configurer cette fonctionnalité.

Pour plus d’informations sur les licences DLP de point de [terminaison, voir Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
