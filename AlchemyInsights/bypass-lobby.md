---
title: Contourner la salle d’entrée
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059594"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Contrôler les paramètres de salle d’Teams

Si vous souhaitez autoriser tout le monde, y compris les utilisateurs de connexion, externes et anonymes, à contourner la salle d’entrée, utilisez PowerShell pour accomplir cette tâche. Voici un exemple de modification de la stratégie de réunion globale pour votre organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cette cmdlet nécessite actuellement l’utilisation de Skype Entreprise module PowerShell. Pour vous configurer pour utiliser cette cmdlet, consultez La gestion des [stratégies via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Une fois que vous avez installé une stratégie, vous devez l’appliquer aux utilisateurs . ou, si vous avez modifié la stratégie globale, elle s’appliquera automatiquement aux utilisateurs. Pour toute modification de stratégie, vous devez attendre au moins 4 heures **jusqu’à 24** heures pour que les stratégies prennent effet. 

Veillez à consulter la documentation ci-dessous avant d’apporter ces modifications pour comprendre exactement ce que cela permet.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Comprendre les contrôles de Teams de salle d’accueil des réunions

Ces paramètres contrôlent les participants à la réunion qui attendent dans la salle d’attente avant d’être admis à la réunion et le niveau de participation qu’ils sont autorisés à participer à une réunion. Vous pouvez utiliser PowerShell pour mettre à jour les paramètres de stratégie de réunion qui n’ont pas encore été implémentés (étiquetés « bientôt ») dans le Centre d’administration Teams. Voir ci-dessous un exemple d’cmdlet PowerShell qui permet à tous les utilisateurs de contourner la salle d’entrée.

- [Admettre automatiquement les](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) personnes est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admis par un utilisateur authentifié.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Autoriser les personnes anonymes à démarrer une réunion est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris les utilisateurs B2B et fédérés, peuvent participer à la réunion de l’utilisateur sans qu’un utilisateur authentifié de l’organisation y participe.

- Autoriser les utilisateurs d’appels [rendez-vous](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) à contourner la salle d’attente **(bientôt** disponible) est une stratégie par  organisateur qui contrôle si les personnes qui appellent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente, quel que soit le paramètre Admettre automatiquement les personnes.

- Autoriser les organisateurs à remplacer les [paramètres](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) de la salle d’accueil **(bientôt** disponible) est une stratégie  par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de salle d’accueil qu’un administrateur a définies dans Admettre automatiquement les personnes et autoriser les utilisateurs à se rendre à la conférence **rendez-vous** à ignorer la salle d’entrée lorsqu’ils organisent une nouvelle réunion.

**Remarque :** Lisez [Gérer les stratégies de réunion dans Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pour une vue d’ensemble complète Microsoft Teams stratégies de réunion.
