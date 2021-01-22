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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917312"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="c1d9d-102">Activer la technologie NDI</span><span class="sxs-lookup"><span data-stu-id="c1d9d-102">Turn on NDI technology</span></span>

<span data-ttu-id="c1d9d-103">La technologie NDI nécessite deux étapes pour être allumée pour un utilisateur :</span><span class="sxs-lookup"><span data-stu-id="c1d9d-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="c1d9d-104">L’administrateur client doit activer la propriété « AllowNDIStreaming » dans CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="c1d9d-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="c1d9d-105">Une fois cette modification remplie, l’utilisateur final doit activer la technologie NDI® pour son client spécifique à partir des **paramètres > autorisations**.</span><span class="sxs-lookup"><span data-stu-id="c1d9d-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="c1d9d-106">Pour plus d’informations, voir [Utiliser la technologie NDI dans Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="c1d9d-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
