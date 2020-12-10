---
title: Chaîne de l’agent utilisateur Microsoft Edge (bureau)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49609613"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="a67f7-102">Chaîne de l’agent utilisateur Microsoft Edge (bureau)</span><span class="sxs-lookup"><span data-stu-id="a67f7-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="a67f7-103">Les chaînes de l’agent utilisateur (UA) permettent de détecter la version d’un navigateur spécifique utilisée sur un certain système d’exploitation.</span><span class="sxs-lookup"><span data-stu-id="a67f7-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="a67f7-104">Comme les autres navigateurs, Microsoft Edge inclut ces informations dans l’en-tête HTTP « User-agent » chaque fois qu’il effectue une demande à un site.</span><span class="sxs-lookup"><span data-stu-id="a67f7-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="a67f7-105">Les informations de version du navigateur sont également accessibles via JavaScript en interrogeant la valeur de « Navigator. userAgent ».</span><span class="sxs-lookup"><span data-stu-id="a67f7-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="a67f7-106">Nous recommandons aux développeurs Web d’utiliser la détection de fonctionnalité chaque fois que cela est possible pour améliorer la facilité de gestion du code, réduire les Fragility de code et éliminer le risque de rupture du code en cas de mise à jour ultérieure des chaînes UA.</span><span class="sxs-lookup"><span data-stu-id="a67f7-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="a67f7-107">Pour plus d’informations, consultez la rubrique [Microsoft Edge user agent String (bureau)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="a67f7-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>