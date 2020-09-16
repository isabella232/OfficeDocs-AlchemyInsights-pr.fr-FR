---
title: CDN utilisé pour la lecture de la vidéo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 6bc87783375a206a84c96eb7ddd58db5bfd31728
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756965"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="38362-102">CDN utilisé pour la lecture de la vidéo</span><span class="sxs-lookup"><span data-stu-id="38362-102">CDN used for video playback</span></span>

<span data-ttu-id="38362-103">Les événements en direct provenant de Stream et d’applications ou d’un appareil externe et les événements en direct de Yammer/Teams utilisent automatiquement Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="38362-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="38362-104">Les vidéos à la demande téléchargées dans Stream n’utilisent pas encore Azure CDN pour la lecture.</span><span class="sxs-lookup"><span data-stu-id="38362-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="38362-105">Les vidéos préenregistrées dans Stream sont lues à partir du serveur d’origine Azure Media Services associé à votre client dans la zone géographique de votre client.</span><span class="sxs-lookup"><span data-stu-id="38362-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="38362-106">Si vous souhaitez en savoir plus, voir : </span><span class="sxs-lookup"><span data-stu-id="38362-106">For more information, see:</span></span>

- [<span data-ttu-id="38362-107">CDN utilisé pour la lecture de la vidéo</span><span class="sxs-lookup"><span data-stu-id="38362-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
