---
title: Paramètres de stratégie de réunion
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794332"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="791c4-102">Gérer les stratégies de réunion dans Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="791c4-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="791c4-103">**Remarque : les modifications apportées aux stratégies peuvent prendre jusqu’à 24 heures pour être appliquées aux utilisateurs.**</span><span class="sxs-lookup"><span data-stu-id="791c4-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="791c4-104">Il se peut que vous ne puissiez pas modifier immédiatement les stratégies nouvellement créées ; Patientez 4 heures et essayez à nouveau de modifier une stratégie nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="791c4-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="791c4-105">Les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles pour les participants à la réunion pour les réunions planifiées par les utilisateurs au sein de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="791c4-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="791c4-106">Certaines fonctionnalités des stratégies de réunion peuvent ne pas être implémentées dans le centre d’administration teams encore (celles-ci sont étiquetées « bientôt disponible » dans la documentation).</span><span class="sxs-lookup"><span data-stu-id="791c4-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="791c4-107">Dans ce cas, ou si vous recevez une erreur de type « nous ne pouvons pas mettre à jour la stratégie pour le moment, mais réessayez plus tard » dans le centre d’administration Microsoft Teams, nous vous recommandons d’utiliser PowerShell pour créer ou modifier des stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="791c4-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="791c4-108">Pour plus d’informations sur les stratégies de réunion, consultez les ressources suivantes :</span><span class="sxs-lookup"><span data-stu-id="791c4-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="791c4-109">Pour en savoir plus sur la création de stratégies, l’apport de modifications et l’affectation d’utilisateurs à la stratégie, consultez la rubrique [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="791c4-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="791c4-110">Pour effectuer des modifications de stratégie à l’aide des cmdlets PowerShell, voir [teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="791c4-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="791c4-111">Vous devez utiliser le [module Skype entreprise PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) pour les stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="791c4-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="791c4-112">Consultez la [documentation des applets de commande \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="791c4-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

