---
title: 'Dépannage de la messagerie vocale '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607998"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="f95c6-102">Dépannage de la messagerie vocale</span><span class="sxs-lookup"><span data-stu-id="f95c6-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="f95c6-103">Assurez-vous que la fonctionnalité Busy on Busy est intentionnelle.</span><span class="sxs-lookup"><span data-stu-id="f95c6-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="f95c6-104">Si cette fonctionnalité n’est pas nécessaire sur cet utilisateur :</span><span class="sxs-lookup"><span data-stu-id="f95c6-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="f95c6-105">Accédez au [Centre d’administration teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="f95c6-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="f95c6-106">Sur le rail gauche, naviguez vers les  >  **stratégies d’appel** vocal  >  **gérer les stratégies** sur la stratégie d' **appel**.</span><span class="sxs-lookup"><span data-stu-id="f95c6-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="f95c6-107">Sélectionnez **gérer les utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="f95c6-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="f95c6-108">Recherchez utilisateur et modifiez la stratégie d’appel de façon à ce qu’elle **soit disponible lorsqu’elle est en cours** d' appel.</span><span class="sxs-lookup"><span data-stu-id="f95c6-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="f95c6-109">Cliquez sur **Appliquer**.</span><span class="sxs-lookup"><span data-stu-id="f95c6-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="f95c6-110">La réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="f95c6-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="f95c6-111">Pour plus d’informations sur cette fonctionnalité, reportez-vous à la rubrique : [Busy on Busy est disponible lors d’un appel](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="f95c6-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
