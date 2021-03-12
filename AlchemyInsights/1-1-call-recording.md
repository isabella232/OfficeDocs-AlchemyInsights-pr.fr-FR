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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733847"
---
# <a name="11-call-recording"></a><span data-ttu-id="6aa31-102">Enregistrement des appels 1:1</span><span class="sxs-lookup"><span data-stu-id="6aa31-102">1:1 call recording</span></span>

<span data-ttu-id="6aa31-103">Les administrateurs doivent prendre des mesures dès maintenant pour continuer à autoriser les utilisateurs à enregistrer les appels 1:1.</span><span class="sxs-lookup"><span data-stu-id="6aa31-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="6aa31-104">À compter du 12 avril 2021, nous allons commencer à appliquer une nouvelle option de stratégie d’appel Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="6aa31-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="6aa31-105">Actuellement, les fonctionnalités d’enregistrement des appels 1:1 sont contrôlées par l’option *AllowCloudRecording* dans les stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="6aa31-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="6aa31-106">Si vos utilisateurs sont autorisés à enregistrer des réunions Teams, ils peuvent également enregistrer des appels 1:1.</span><span class="sxs-lookup"><span data-stu-id="6aa31-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="6aa31-107">Si vous préférez empêcher tous les utilisateurs d’enregistrer des appels 1:1, aucune action n’est nécessaire.</span><span class="sxs-lookup"><span data-stu-id="6aa31-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="6aa31-108">L’option de stratégie d’appel *AllowCloudRecordingForCalls* sera $False par défaut.</span><span class="sxs-lookup"><span data-stu-id="6aa31-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="6aa31-109">Cette modification est documentée dans la publication suivante du Centre de messages : (Mise à [jour) 1:1 Introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) de la stratégie d’enregistrement des appels pour définir l’option de stratégie d’appel Teams, vous devez utiliser Teams [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="6aa31-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="6aa31-110">Pour activer l’enregistrement des appels dans les appels **1:1** : Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="6aa31-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="6aa31-111">Pour désactiver l’enregistrement des appels dans les appels **1:1** : Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="6aa31-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

