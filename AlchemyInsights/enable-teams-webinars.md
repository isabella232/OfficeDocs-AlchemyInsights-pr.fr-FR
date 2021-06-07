---
title: Activer les webinaires Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760835"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="1d544-102">Activer les webinaires Teams</span><span class="sxs-lookup"><span data-stu-id="1d544-102">Enable Teams Webinars</span></span>

<span data-ttu-id="1d544-103">Les webinaires sont activés par défaut.</span><span class="sxs-lookup"><span data-stu-id="1d544-103">Webinars are enabled by default.</span></span> <span data-ttu-id="1d544-104">Vous pouvez gérer qui peut planifier et s’inscrire aux webinaires Teams à l’aide des commandes Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1d544-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="1d544-105">Tous les utilisateurs qui peuvent créer une réunion peuvent également créer une réunion de webinaires.</span><span class="sxs-lookup"><span data-stu-id="1d544-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="1d544-106">Si vous souhaitez gérer qui peut planifier des webinaires Teams, utilisez *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="1d544-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="1d544-107">Par défaut,  WhoCanRegister est activé et défini sur **Tout le monde**.</span><span class="sxs-lookup"><span data-stu-id="1d544-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="1d544-108">Si vous souhaitez désactiver l’inscription à la réunion, définissez *AllowMeetingRegistration* sur **False**.</span><span class="sxs-lookup"><span data-stu-id="1d544-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="1d544-109">Pour modifier ces paramètres, vous devez installer [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="1d544-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="1d544-110">En outre, les stratégies de réunion sont appliquées aux webinaires Teams.</span><span class="sxs-lookup"><span data-stu-id="1d544-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="1d544-111">Par exemple, si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires.</span><span class="sxs-lookup"><span data-stu-id="1d544-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="1d544-112">Pour en savoir plus sur la configuration de qui peut s’inscrire aux webinaires, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="1d544-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="1d544-113">Pour plus d’informations sur les paramètres des listes Microsoft, consultez [Paramètres de contrôle pour Listes Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="1d544-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>