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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704604"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="abd7d-102">Gérer les stratégies de réunion dans Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="abd7d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="abd7d-103">**Remarque : l’application des modifications de stratégie pour les utilisateurs peut prendre jusqu’à 24 heures.**</span><span class="sxs-lookup"><span data-stu-id="abd7d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="abd7d-104">Il se peut que vous ne soyez pas en mesure d’apporter des modifications immédiatement aux stratégies nouvellement créées ; patientez 4 heures et tentez à nouveau de modifier une stratégie nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="abd7d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="abd7d-105">Les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles pour les participants aux réunions qui sont prévues par les utilisateurs de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="abd7d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="abd7d-106">Certaines fonctionnalités des stratégies de réunion peuvent ne pas encore être implémentées dans le Centre d’administration Teams (celles-ci sont étiquetées « prochainement » dans la documentation).</span><span class="sxs-lookup"><span data-stu-id="abd7d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="abd7d-107">Dans ce cas, ou si vous êtes en train d’obtenir une erreur telle que « Nous ne pouvons pas mettre à jour la stratégie pour le moment, mais essayer à nouveau plus tard » dans le Centre d’administration Microsoft Teams, nous vous recommandons d’utiliser PowerShell pour créer ou modifier des stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="abd7d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="abd7d-108">Pour plus d’informations sur les stratégies de réunion, consultez les ressources suivantes :</span><span class="sxs-lookup"><span data-stu-id="abd7d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="abd7d-109">Pour en savoir plus sur la création de stratégies, la modification et l’affectation d’utilisateurs à la stratégie, voir Gérer les stratégies [de réunion dans Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="abd7d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="abd7d-110">Pour apporter des modifications de stratégie à l’aide des cmdlets PowerShell, voir [Vue d’ensemble de Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="abd7d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="abd7d-111">Vous devez utiliser le [module PowerShell Skype Entreprise](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) pour les stratégies de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="abd7d-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="abd7d-112">Pour plus d’informations, veuillez consulter la documentation des [cmdlets \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="abd7d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

