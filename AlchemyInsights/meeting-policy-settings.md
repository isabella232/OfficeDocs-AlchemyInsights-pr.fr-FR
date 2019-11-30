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
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gérer les stratégies de réunion dans Microsoft teams

Les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles pour les participants à la réunion pour les réunions planifiées par les utilisateurs au sein de votre organisation. Certaines fonctionnalités des stratégies de réunion peuvent ne pas être implémentées dans le centre d’administration teams encore (celles-ci sont étiquetées « bientôt disponible » dans la documentation). Dans ce cas, ou si vous recevez une erreur de type « nous ne pouvons pas mettre à jour la stratégie pour le moment, mais réessayez plus tard » dans le centre d’administration Microsoft Teams, nous vous recommandons d’utiliser PowerShell pour créer ou modifier des stratégies de réunion Teams. 

Pour plus d’informations sur les stratégies de réunion, consultez les ressources suivantes :

- Pour en savoir plus sur la création de stratégies, l’apport de modifications et l’affectation d’utilisateurs à la stratégie, consultez la rubrique [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pour effectuer des modifications de stratégie à l’aide des cmdlets PowerShell, voir [teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Vous devez utiliser le [module Skype entreprise PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) pour les stratégies de réunion Teams. 
    - Consultez la [documentation des applets de commande *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pour plus d’informations.

**Remarque :** L’application des modifications de stratégie pour les utilisateurs peut prendre jusqu’à 24 heures. Il se peut que vous ne puissiez pas modifier immédiatement les stratégies nouvellement créées ; Patientez 4 heures et essayez à nouveau de modifier une stratégie nouvellement créée. Si vous rencontrez toujours des problèmes, essayez PowerShell.  