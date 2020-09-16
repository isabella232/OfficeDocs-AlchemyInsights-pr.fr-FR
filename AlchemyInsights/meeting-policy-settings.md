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
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gérer les stratégies de réunion dans Microsoft teams

**Remarque : les modifications apportées aux stratégies peuvent prendre jusqu’à 24 heures pour être appliquées aux utilisateurs.** Il se peut que vous ne puissiez pas modifier immédiatement les stratégies nouvellement créées ; Patientez 4 heures et essayez à nouveau de modifier une stratégie nouvellement créée.

Les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles pour les participants à la réunion pour les réunions planifiées par les utilisateurs au sein de votre organisation. Certaines fonctionnalités des stratégies de réunion peuvent ne pas être implémentées dans le centre d’administration teams encore (celles-ci sont étiquetées « bientôt disponible » dans la documentation). Dans ce cas, ou si vous recevez une erreur de type « nous ne pouvons pas mettre à jour la stratégie pour le moment, mais réessayez plus tard » dans le centre d’administration Microsoft Teams, nous vous recommandons d’utiliser PowerShell pour créer ou modifier des stratégies de réunion Teams. 

Pour plus d’informations sur les stratégies de réunion, consultez les ressources suivantes :

- Pour en savoir plus sur la création de stratégies, l’apport de modifications et l’affectation d’utilisateurs à la stratégie, consultez la rubrique [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pour effectuer des modifications de stratégie à l’aide des cmdlets PowerShell, voir [teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Vous devez utiliser le [module Skype entreprise PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) pour les stratégies de réunion Teams. 
    - Consultez la [documentation des applets de commande *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pour plus d’informations.

