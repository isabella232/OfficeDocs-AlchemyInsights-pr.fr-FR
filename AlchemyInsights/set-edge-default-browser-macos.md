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
ms.openlocfilehash: e04f8931ef12c426a5c3d5f617fc5f5d5c3a15c6fe43f7b84a7e97e8ee04e3fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073958"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Définir Microsoft Edge comme navigateur par défaut sur un appareil macOS

Utilisez l’une de ces deux méthodes pour définir Microsoft Edge comme navigateur par défaut :

Méthode 1 : flashez l’appareil avec une image de macOS dans laquelle Microsoft Edge a déjà été définie comme navigateur par défaut.

Méthode 2 : définissez la stratégie DefaultBrowserSettingEnabled pour inviter l’utilisateur à définir Microsoft Edge comme navigateur par défaut.

L’une ou l’autre méthode permet à un utilisateur de changer le navigateur par défaut. Pour cette raison, nous vous recommandons de déployer la stratégie DefaultBrowserSettingEnabled même si vous avez utilisé la méthode 1. Si un utilisateur change le navigateur par défaut après le déploiement de la stratégie, la stratégie invite l’utilisateur à définir de nouveau le navigateur par défaut sur Microsoft Edge.
