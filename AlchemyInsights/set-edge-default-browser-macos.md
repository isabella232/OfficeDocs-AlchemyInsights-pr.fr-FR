---
title: Définir Microsoft Edge comme navigateur par défaut sur un appareil macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426788"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Définir Microsoft Edge comme navigateur par défaut sur un appareil macOS

Utilisez l’une de ces deux méthodes pour définir Microsoft Edge comme navigateur par défaut :

Méthode 1 : flashez l’appareil avec une image de macOS dans laquelle Microsoft Edge a déjà été définie comme navigateur par défaut.

Méthode 2 : définissez la stratégie DefaultBrowserSettingEnabled pour inviter l’utilisateur à définir Microsoft Edge comme navigateur par défaut.

L’une ou l’autre méthode permet à un utilisateur de changer le navigateur par défaut. Pour cette raison, nous vous recommandons de déployer la stratégie DefaultBrowserSettingEnabled même si vous avez utilisé la méthode 1. Si un utilisateur change le navigateur par défaut après le déploiement de la stratégie, la stratégie invite l’utilisateur à définir de nouveau le navigateur par défaut sur Microsoft Edge.
