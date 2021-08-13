---
title: Microsoft Edge de l’agent utilisateur (Bureau)
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
ms.openlocfilehash: 9311f17298fff3fee3282fe05bd1ddcd02780a80097e86b29d56ffd575a9a571
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975999"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Microsoft Edge de l’agent utilisateur (Bureau)

Les chaînes de l’agent utilisateur peuvent être utilisées pour détecter la version d’un navigateur spécifique utilisée sur un certain système d’exploitation. Comme d’autres navigateurs, Microsoft Edge inclut ces informations dans l’en-tête HTTP « Agent utilisateur » chaque fois qu’il effectue une demande d’accès à un site. Les informations sur la version du navigateur sont également accessibles via JavaScript en interrogeant la valeur de « navigator.userAgent ».

Nous recommandons aux développeurs web d'utiliser la détection des fonctionnalités chaque fois que possible afin d'améliorer la maintenabilité du code, de réduire sa fragilité et d'éliminer le risque de rupture du code en cas de futures mises à jour de la chaîne de l'agent utilisateur.

Pour plus d’informations, consultez [Chaîne de l'agent utilisateur de Microsoft Edge (Bureau)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).