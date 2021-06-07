---
title: Gérer l’inscription au webinaire
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
- "11512"
- "9006672"
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760831"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="2e9ff-102">Gérer l’inscription au webinaire</span><span class="sxs-lookup"><span data-stu-id="2e9ff-102">Manage webinar registration</span></span>

<span data-ttu-id="2e9ff-103">Vous pouvez gérer qui peut s’inscrire aux webinaires Teams à l’aide des commandes Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2e9ff-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="2e9ff-104">Par défaut,  WhoCanRegister est activé et défini sur **Tout le monde**.</span><span class="sxs-lookup"><span data-stu-id="2e9ff-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="2e9ff-105">Si vous souhaitez désactiver l’inscription à la réunion, définissez *AllowMeetingRegistration* sur **False**.</span><span class="sxs-lookup"><span data-stu-id="2e9ff-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2e9ff-106">Pour modifier ces paramètres, vous devez installer [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="2e9ff-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="2e9ff-107">En outre, les stratégies de réunion sont appliquées aux webinaires Teams.</span><span class="sxs-lookup"><span data-stu-id="2e9ff-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="2e9ff-108">Par exemple, si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires.</span><span class="sxs-lookup"><span data-stu-id="2e9ff-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="2e9ff-109">Pour en savoir plus sur la configuration de qui peut s’inscrire aux webinaires, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="2e9ff-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2e9ff-110">Pour plus d’informations sur les paramètres des listes Microsoft, consultez [Paramètres de contrôle pour Listes Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="2e9ff-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>