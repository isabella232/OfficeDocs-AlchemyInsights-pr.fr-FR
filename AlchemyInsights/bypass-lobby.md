---
title: En-salle de dérivation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626346"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Paramètres de la salle d’attente de contrôle et niveau de participation

Si vous souhaitez autoriser tout le monde, y compris les utilisateurs d’appels entrants, externes et anonymes à contourner la salle d’attente dans Microsoft Teams, vous pouvez utiliser PowerShell pour effectuer cette tâche. Voici un exemple de modification de la stratégie de réunion globale pour votre organisation :

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cette applet de commande requiert actuellement l’utilisation du module Skype entreprise PowerShell. Pour obtenir le programme d’installation de cette cmdlet, consultez la rubrique [gestion des stratégies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Vous pouvez configurer une nouvelle stratégie, que vous devrez ensuite appliquer à vos utilisateurs. Si vous modifiez la stratégie globale, elle s’applique automatiquement aux utilisateurs. Pour toute modification de stratégie, vous devez attendre au moins 4 heures et jusqu’à 24 heures pour que les stratégies prennent effet.

Veillez à consulter la documentation ci-dessous avant de faire en sorte que ces modifications comprennent exactement ce que cela autorise.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Présentation des contrôles de stratégie de salle d’attente de réunion teams

- L' [admission automatique des personnes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admises par un utilisateur authentifié.

- [Autoriser les utilisateurs anonymes à démarrer une réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris B2B et les utilisateurs fédérés, peuvent rejoindre la réunion sans utilisateur authentifié de l’organisation en participation.

- Autoriser les utilisateurs de rendez [-vous à contourner le lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si les personnes qui se connectent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente indépendamment du paramètre **autoriser les personnes automatiquement** .

- [Permettre aux organisateurs de remplacer les paramètres de la salle d’attente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de la salle d’attente qu’un administrateur a défini de manière à **admettre automatiquement les personnes** et permettre aux utilisateurs de rendez **-vous de contourner la salle d’attente** lorsqu’ils planifient une nouvelle réunion.

**Remarque :** Consultez [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pour obtenir une vue d’ensemble des stratégies de réunion Microsoft Teams.
