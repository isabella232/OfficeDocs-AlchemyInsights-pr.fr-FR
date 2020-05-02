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
# <a name="private-channels-in-microsoft-teams"></a>Canaux privés dans Microsoft teams

Les canaux privés sont une nouvelle fonctionnalité de Microsoft Teams. Notez que les canaux privés ne peuvent pas être convertis à partir de canaux standard ou vice versa.

Pour plus d’informations sur les canaux privés, tels que les informations sur la [création de canal privé, l’appartenance](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) et les [sites SharePoint de canal privé](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), consultez la rubrique [Private Channels in Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Remarque :** Étant donné que la configuration de la rétention des messages de canal privé n’est pas encore prise en charge, les clients avec des stratégies de rétention activées n’auront pas de canaux privés activés par défaut. Les canaux privés peuvent être activés dans le centre d’administration Teams. Notez également que si la rétention des messages de canal privé n’est pas prise en charge, la rétention des fichiers partagés dans les canaux privés est prise en charge.

**Vous avez besoin d’un nouveau propriétaire d’équipe ?**

Si le propriétaire de votre canal privé laisse, vous pouvez ajouter un nouveau propriétaire d’équipe via PowerShell PowerShell.


- Accédez [ici](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) pour installer teams PowerShell.

Voici la cmdlet dont vous aurez besoin :

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Pour plus d’informations sur PowerShell Teams, reportez-vous à [teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
