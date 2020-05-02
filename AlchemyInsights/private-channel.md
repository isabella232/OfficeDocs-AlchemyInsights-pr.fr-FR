---
title: Canal privé
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005436"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="bc243-102">Canaux privés dans Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="bc243-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="bc243-103">Les canaux privés sont une nouvelle fonctionnalité de Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bc243-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="bc243-104">Notez que les canaux privés ne peuvent pas être convertis à partir de canaux standard ou vice versa.</span><span class="sxs-lookup"><span data-stu-id="bc243-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="bc243-105">Pour plus d’informations sur les canaux privés, tels que les informations sur la [création de canal privé, l’appartenance](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) et les [sites SharePoint de canal privé](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), consultez la rubrique [Private Channels in Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="bc243-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="bc243-106">**Remarque :** Étant donné que la configuration de la rétention des messages de canal privé n’est pas encore prise en charge, les clients avec des stratégies de rétention activées n’auront pas de canaux privés activés par défaut.</span><span class="sxs-lookup"><span data-stu-id="bc243-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="bc243-107">Les canaux privés peuvent être activés dans le centre d’administration Teams.</span><span class="sxs-lookup"><span data-stu-id="bc243-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="bc243-108">Notez également que si la rétention des messages de canal privé n’est pas prise en charge, la rétention des fichiers partagés dans les canaux privés est prise en charge.</span><span class="sxs-lookup"><span data-stu-id="bc243-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="bc243-109">**Vous avez besoin d’un nouveau propriétaire d’équipe ?**</span><span class="sxs-lookup"><span data-stu-id="bc243-109">**Need a new team owner?**</span></span>

<span data-ttu-id="bc243-110">Si le propriétaire de votre canal privé laisse, vous pouvez ajouter un nouveau propriétaire d’équipe via PowerShell PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bc243-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="bc243-111">Accédez [ici](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) pour installer teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bc243-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="bc243-112">Voici la cmdlet dont vous aurez besoin :</span><span class="sxs-lookup"><span data-stu-id="bc243-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="bc243-113">Pour plus d’informations sur PowerShell Teams, reportez-vous à [teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="bc243-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
