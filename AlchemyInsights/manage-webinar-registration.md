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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798642"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="28db6-102">Gérer l’inscription au webinaire</span><span class="sxs-lookup"><span data-stu-id="28db6-102">Manage webinar registration</span></span>

<span data-ttu-id="28db6-103">Vous pouvez gérer qui peut s’inscrire aux webinaires Teams à l’aide des commandes Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28db6-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="28db6-104">Pour installer Teams PowerShell, consultez [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="28db6-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="28db6-105">Par défaut, *WhoCanRegister* est activé et défini sur **Tout le monde**.</span><span class="sxs-lookup"><span data-stu-id="28db6-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="28db6-106">Si vous ne voyez pas l’option permettant d’autoriser l’inscription à Tout le monde dans l’invitation à la réunion, réexécutez le paramètre *WhoCanRegister* à Tout le monde et attendez 24 heures.</span><span class="sxs-lookup"><span data-stu-id="28db6-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="28db6-107">Pour réexécuter *WhoCanRegister*, utilisez la commande PowerShell :</span><span class="sxs-lookup"><span data-stu-id="28db6-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="28db6-108">**Remarque**: si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires.</span><span class="sxs-lookup"><span data-stu-id="28db6-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="28db6-109">Pour en savoir plus et activer ce paramètre, consultez [Gérer les paramètres de réunion dans Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="28db6-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="28db6-110">Si vous souhaitez désactiver l’inscription à la réunion, définissez *AllowMeetingRegistration* sur **False**.</span><span class="sxs-lookup"><span data-stu-id="28db6-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="28db6-111">Pour en savoir plus sur la configuration de qui peut s’inscrire aux webinaires, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="28db6-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="28db6-112">Pour plus d’informations sur les paramètres des listes Microsoft, consultez [Paramètres de contrôle pour Listes Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="28db6-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
