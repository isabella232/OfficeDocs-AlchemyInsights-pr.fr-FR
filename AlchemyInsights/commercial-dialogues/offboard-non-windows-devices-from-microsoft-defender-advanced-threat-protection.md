---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735927"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="57099-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="57099-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="57099-103">Voici comment procéder :</span><span class="sxs-lookup"><span data-stu-id="57099-103">Here's how:</span></span>

1. <span data-ttu-id="57099-104">Suivez la documentation tierce pour déconnecter la solution tierce de Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="57099-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="57099-105">À partir de votre client Azure Active Directory, supprimez les autorisations pour la solution tierce :</span><span class="sxs-lookup"><span data-stu-id="57099-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="57099-106">Connectez-vous au [portail Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="57099-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="57099-107">Sélectionnez **tous les services** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="57099-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="57099-108">Sélectionnez l’application que vous souhaitez horsboard.</span><span class="sxs-lookup"><span data-stu-id="57099-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="57099-109">Sélectionnez **Supprimer**.</span><span class="sxs-lookup"><span data-stu-id="57099-109">Select **Delete**.</span></span>

<span data-ttu-id="57099-110">Pour en savoir plus, consultez [Les appareils hors](https://go.microsoft.com/fwlink/?linkid=2143630)Windows.</span><span class="sxs-lookup"><span data-stu-id="57099-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
