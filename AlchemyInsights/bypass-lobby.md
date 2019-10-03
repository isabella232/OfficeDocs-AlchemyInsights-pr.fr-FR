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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376633"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Paramètres de la salle d’attente de contrôle et niveau de participation

Ces paramètres contrôlent les participants à la réunion qui attendent dans la salle d’attente avant d’être admis à la réunion et le niveau de participation qu’ils sont autorisés à participer à une réunion. Vous pouvez utiliser PowerShell pour mettre à jour les paramètres de stratégie de réunion qui n’ont pas encore été mis en œuvre (étiqueté « bientôt disponible ») dans le centre d’administration Teams.  Voir ci-dessous un exemple d’applet de commande PowerShell qui permet à tous les utilisateurs de contourner la salle d’attente.  

- L' [admission automatique des personnes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admises par un utilisateur authentifié.

- [Autoriser les utilisateurs anonymes à démarrer une réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris B2B et les utilisateurs fédérés, peuvent rejoindre la réunion sans utilisateur authentifié de l’organisation en participation.

- Autoriser les utilisateurs de rendez [-vous à contourner le lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si les personnes qui se connectent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente indépendamment du paramètre **autoriser les personnes automatiquement** .

- [Permettre aux organisateurs de remplacer les paramètres de la salle d’attente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de la salle d’attente qu’un administrateur a défini de manière à **admettre automatiquement les personnes** et **à autoriser les appels entrants utilisateurs à contourner la salle d’attente** lorsqu’ils planifient une nouvelle réunion.

**Remarque :** Consultez [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pour obtenir une vue d’ensemble des stratégies de réunion Microsoft Teams. 


**Exemple PowerShell**

Si vous souhaitez autoriser tout le monde, y compris les utilisateurs externes ou anonymes, à contourner la salle d’attente, vous pouvez également utiliser PowerShell pour accomplir cette tâche.  Voici un exemple de modification de la stratégie de réunion globale pour votre organisation.   

(Veillez à consulter la documentation ci-dessus avant de faire en sorte que ces modifications comprennent exactement ce que cela autorise.)

Set-CsTeamsMeetingPolicy-Identity global-AutoAdmittedUsers « tout le monde »-AllowPSTNUsersToBypassLobby $True

Pour plus d’informations, consultez la rubrique [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
