---
title: En-salle de dérivation
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684948"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Contrôler les paramètres de la salle d’attente et le niveau de participation dans teams

Si vous souhaitez autoriser tout le monde, y compris les utilisateurs d’appels entrants, externes et anonymes, à **contourner la salle d’attente**, utilisez PowerShell pour accomplir cette tâche. Voici un exemple de modification de la stratégie de réunion globale pour votre organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cette applet de commande requiert actuellement l’utilisation du module Skype entreprise PowerShell. Pour configurer l’utilisation de cette cmdlet, consultez la rubrique [gestion des stratégies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Une fois que vous avez configuré une stratégie, vous devez l’appliquer aux utilisateurs ; ou, si vous avez modifié la stratégie globale, elle s’applique automatiquement aux utilisateurs. Pour toute modification de stratégie, vous devez attendre au moins **4 heures jusqu’à 24 heures** pour que les stratégies prennent effet. 

Veillez à consulter la documentation ci-dessous avant de faire en sorte que ces modifications comprennent exactement ce que cela autorise.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Présentation des contrôles de stratégie de salle d’attente de réunion teams

Ces paramètres contrôlent les participants à la réunion qui attendent dans la salle d’attente avant d’être admis à la réunion et le niveau de participation qu’ils sont autorisés à participer à une réunion. Vous pouvez utiliser PowerShell pour mettre à jour les paramètres de stratégie de réunion qui n’ont pas encore été mis en œuvre (étiqueté « bientôt disponible ») dans le centre d’administration Teams. Voir ci-dessous un exemple d’applet de commande PowerShell qui permet à tous les utilisateurs de contourner la salle d’attente.

- L' [admission automatique des personnes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admises par un utilisateur authentifié.

- [Autoriser les utilisateurs anonymes à démarrer une réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris B2B et les utilisateurs fédérés, peuvent rejoindre la réunion sans utilisateur authentifié de l’organisation en participation.

- Autoriser les utilisateurs de rendez [-vous à contourner le lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si les personnes qui se connectent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente indépendamment du paramètre **autoriser les personnes automatiquement** .

- [Permettre aux organisateurs de remplacer les paramètres de la salle d’attente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de la salle d’attente qu’un administrateur a défini de manière à **admettre automatiquement les personnes** et permettre aux utilisateurs de rendez **-vous de contourner la salle d’attente** lorsqu’ils planifient une nouvelle réunion.

**Remarque :** Consultez [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pour obtenir une vue d’ensemble des stratégies de réunion Microsoft Teams.
