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
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="5175b-102">Définir Microsoft Edge comme navigateur par défaut sur un appareil macOS</span><span class="sxs-lookup"><span data-stu-id="5175b-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="5175b-103">Utilisez l’une de ces deux méthodes pour définir Microsoft Edge comme navigateur par défaut :</span><span class="sxs-lookup"><span data-stu-id="5175b-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="5175b-104">Méthode 1 : flashez l’appareil avec une image de macOS dans laquelle Microsoft Edge a déjà été définie comme navigateur par défaut.</span><span class="sxs-lookup"><span data-stu-id="5175b-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="5175b-105">Méthode 2 : définissez la stratégie DefaultBrowserSettingEnabled pour inviter l’utilisateur à définir Microsoft Edge comme navigateur par défaut.</span><span class="sxs-lookup"><span data-stu-id="5175b-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="5175b-106">L’une ou l’autre méthode permet à un utilisateur de changer le navigateur par défaut.</span><span class="sxs-lookup"><span data-stu-id="5175b-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="5175b-107">Pour cette raison, nous vous recommandons de déployer la stratégie DefaultBrowserSettingEnabled même si vous avez utilisé la méthode 1.</span><span class="sxs-lookup"><span data-stu-id="5175b-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="5175b-108">Si un utilisateur change le navigateur par défaut après le déploiement de la stratégie, la stratégie invite l’utilisateur à définir de nouveau le navigateur par défaut sur Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5175b-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
