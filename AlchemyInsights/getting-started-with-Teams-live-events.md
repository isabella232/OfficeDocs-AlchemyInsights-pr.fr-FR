---
title: Prise en main des événements en direct Teams
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
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677277"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="3788a-102">Prise en main des événements en direct Teams</span><span class="sxs-lookup"><span data-stu-id="3788a-102">Getting started with Teams live events</span></span>

<span data-ttu-id="3788a-103">Les événements en direct Microsoft Teams sont une extension des réunions Teams qui vous permettent de planifier et de créer des événements qui sont diffusés à de larges audiences en ligne.</span><span class="sxs-lookup"><span data-stu-id="3788a-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="3788a-104">Pour créer un événement en direct, vous devez disposer des éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="3788a-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="3788a-105">Tout d’abord, assurez-vous que les événements en direct Teams sont [dans votre pays/région](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Les événements en direct ne sont pas encore pris en charge dans certains pays.</span><span class="sxs-lookup"><span data-stu-id="3788a-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="3788a-106">Si vous avez attribué des licences et défini les stratégies, mais que vous ne parvenez pas à créer un événement en direct Teams, il est probable que vous vous trouviez dans un pays ou une région dans lequel les événements en direct ne sont pas encore disponibles.</span><span class="sxs-lookup"><span data-stu-id="3788a-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="3788a-107">Une [licence Office 365 Entreprise E1, E3 ou E5, ou une licence Office 365 A3 ou A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="3788a-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="3788a-108">**Remarque** : en raison d’une hausse récente de l’utilisation de Teams, lorsque vous attribuez une licence Teams à un utilisateur, sa configuration complète peut prendre environ 24 heures.</span><span class="sxs-lookup"><span data-stu-id="3788a-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="3788a-109">En attendant, vous ne serez pas en mesure d’affecter des stratégies Teams à celui-ci, et il ne pourra peut-être pas accéder à certaines fonctionnalités de Teams telles que l’appel et l’audioconférence.</span><span class="sxs-lookup"><span data-stu-id="3788a-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="3788a-110">L’autorisation de [créer des événements en direct dans le centre d’administration Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)</span><span class="sxs-lookup"><span data-stu-id="3788a-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="3788a-111">L’autorisation de [créer des événements en direct dans Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (pour les événements générés à l’aide d’une application ou d’un appareil de diffusion externe)</span><span class="sxs-lookup"><span data-stu-id="3788a-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="3788a-112">Appartenance complète à une équipe au sein de l’organisation (vous ne pouvez pas être un invité ou une autre organisation)</span><span class="sxs-lookup"><span data-stu-id="3788a-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="3788a-113">Planification des réunions privées, ainsi que partage d’écran et de vidéos IP, activés dans la stratégie de réunion d’équipe</span><span class="sxs-lookup"><span data-stu-id="3788a-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="3788a-114">[Meilleures pratiques](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) pour les événements en direct Teams.</span><span class="sxs-lookup"><span data-stu-id="3788a-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="3788a-115">Pour plus d’informations, voir [Prise en main des événements en direct Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="3788a-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>