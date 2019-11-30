---
title: Paramètres de stratégie de réunion
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627572"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6adf9-102">Gérer les stratégies de réunion dans Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="6adf9-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6adf9-103">Les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles pour les participants à la réunion pour les réunions planifiées par les utilisateurs au sein de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="6adf9-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6adf9-104">Certaines fonctionnalités des stratégies de réunion peuvent ne pas être implémentées dans le centre d’administration teams encore (celles-ci sont étiquetées « bientôt disponible » dans la documentation).</span><span class="sxs-lookup"><span data-stu-id="6adf9-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6adf9-105">Dans ce cas, ou si vous recevez une erreur de type « nous ne pouvons pas mettre à jour la stratégie pour le moment, mais réessayez plus tard » dans le centre d’administration Microsoft Teams, nous vous recommandons d’utiliser PowerShell pour créer ou modifier des stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="6adf9-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6adf9-106">Pour plus d’informations sur les stratégies de réunion, consultez les ressources suivantes :</span><span class="sxs-lookup"><span data-stu-id="6adf9-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6adf9-107">Pour en savoir plus sur la création de stratégies, l’apport de modifications et l’affectation d’utilisateurs à la stratégie, consultez la rubrique [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6adf9-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6adf9-108">Pour effectuer des modifications de stratégie à l’aide des cmdlets PowerShell, voir [teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="6adf9-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6adf9-109">Vous devez utiliser le [module Skype entreprise PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) pour les stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="6adf9-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6adf9-110">Consultez la [documentation des applets de commande \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="6adf9-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="6adf9-111">**Remarque :** L’application des modifications de stratégie pour les utilisateurs peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="6adf9-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="6adf9-112">Il se peut que vous ne puissiez pas modifier immédiatement les stratégies nouvellement créées ; Patientez 4 heures et essayez à nouveau de modifier une stratégie nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="6adf9-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="6adf9-113">Si vous rencontrez toujours des problèmes, essayez PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6adf9-113">If you're still having problems, try PowerShell.</span></span>  