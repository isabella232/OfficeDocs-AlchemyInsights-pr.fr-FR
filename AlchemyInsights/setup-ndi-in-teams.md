---
title: Activer la technologie NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023520"
---
# <a name="turn-on-ndi-technology"></a>Activer la technologie NDI

La technologie NDI nécessite deux étapes pour être allumée pour un utilisateur :

1. L’administrateur client doit activer la propriété « AllowNDIStreaming » dans CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Une fois cette modification remplie, l’utilisateur final doit activer la technologie NDI® pour son client spécifique à partir Paramètres > **autorisations.**

Pour plus d’informations, [voir Utiliser la technologie NDI dans Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
