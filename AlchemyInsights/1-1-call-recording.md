---
title: Enregistrement des appels 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696921"
---
# <a name="11-call-recording"></a><span data-ttu-id="186ae-102">Enregistrement des appels 1:1</span><span class="sxs-lookup"><span data-stu-id="186ae-102">1:1 call recording</span></span>

<span data-ttu-id="186ae-103">Si le **bouton Démarrer** l’enregistrement est grisé dans un appel 1:1, vous devez modifier les paramètres de stratégie pour l’utilisateur touché.</span><span class="sxs-lookup"><span data-stu-id="186ae-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="186ae-104">À compter du 31 mai 2021, nous allons commencer à appliquer une nouvelle stratégie d’appel Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="186ae-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="186ae-105">Avant cette modification, l’enregistrement des appels 1:1 est contrôlé par la stratégie de réunion Teams *AllowCloudRecording.*</span><span class="sxs-lookup"><span data-stu-id="186ae-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="186ae-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="186ae-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="186ae-107">*AllowCloudRecordingForCalls*   L’option de stratégie d’appel **est $False** par défaut.</span><span class="sxs-lookup"><span data-stu-id="186ae-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="186ae-108">Si vous préférez empêcher tous les utilisateurs d’enregistrer des appels 1:1, aucune action n’est nécessaire.</span><span class="sxs-lookup"><span data-stu-id="186ae-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="186ae-109">Pour activer l’enregistrement des appels pour tous les utilisateurs dans les appels 1:1, utilisez Teams PowerShell pour exécuter l’cmdlet suivante :</span><span class="sxs-lookup"><span data-stu-id="186ae-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="186ae-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="186ae-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="186ae-111">Vous pouvez également créer une stratégie et définir **-AllowCloudRecordingForCalls** sur **$true** et affecter cette stratégie à vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="186ae-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="186ae-112">Pour plus d’informations, voir [1:1 Call Recording Policy Controls Are (Almost!) Ici](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="186ae-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
