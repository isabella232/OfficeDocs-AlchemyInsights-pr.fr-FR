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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="06fa6-102">Paramètres de la salle d’attente de contrôle et niveau de participation</span><span class="sxs-lookup"><span data-stu-id="06fa6-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="06fa6-103">Ces paramètres contrôlent les participants à la réunion qui attendent dans la salle d’attente avant d’être admis à la réunion et le niveau de participation qu’ils sont autorisés à participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="06fa6-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="06fa6-104">Vous pouvez utiliser PowerShell pour mettre à jour les paramètres de stratégie de réunion qui n’ont pas encore été mis en œuvre (étiqueté « bientôt disponible ») dans le centre d’administration Teams.</span><span class="sxs-lookup"><span data-stu-id="06fa6-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="06fa6-105">Voir ci-dessous un exemple d’applet de commande PowerShell qui permet à tous les utilisateurs de contourner la salle d’attente.</span><span class="sxs-lookup"><span data-stu-id="06fa6-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="06fa6-106">L' [admission automatique des personnes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admises par un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="06fa6-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="06fa6-107">[Autoriser les utilisateurs anonymes à démarrer une réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris B2B et les utilisateurs fédérés, peuvent rejoindre la réunion sans utilisateur authentifié de l’organisation en participation.</span><span class="sxs-lookup"><span data-stu-id="06fa6-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="06fa6-108">Autoriser les utilisateurs de rendez [-vous à contourner le lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si les personnes qui se connectent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente indépendamment du paramètre **autoriser les personnes automatiquement** .</span><span class="sxs-lookup"><span data-stu-id="06fa6-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="06fa6-109">[Permettre aux organisateurs de remplacer les paramètres de la salle d’attente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de la salle d’attente qu’un administrateur a défini de manière à **admettre automatiquement les personnes** et **à autoriser les appels entrants utilisateurs à contourner la salle d’attente** lorsqu’ils planifient une nouvelle réunion.</span><span class="sxs-lookup"><span data-stu-id="06fa6-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="06fa6-110">**Remarque :** Consultez [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pour obtenir une vue d’ensemble des stratégies de réunion Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="06fa6-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="06fa6-111">**Exemple PowerShell**</span><span class="sxs-lookup"><span data-stu-id="06fa6-111">**PowerShell example**</span></span>

<span data-ttu-id="06fa6-112">Si vous souhaitez autoriser tout le monde, y compris les utilisateurs externes ou anonymes, à contourner la salle d’attente, vous pouvez également utiliser PowerShell pour accomplir cette tâche.</span><span class="sxs-lookup"><span data-stu-id="06fa6-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="06fa6-113">Voici un exemple de modification de la stratégie de réunion globale pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="06fa6-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="06fa6-114">(Veillez à consulter la documentation ci-dessus avant de faire en sorte que ces modifications comprennent exactement ce que cela autorise.)</span><span class="sxs-lookup"><span data-stu-id="06fa6-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="06fa6-115">Set-CsTeamsMeetingPolicy-Identity global-AutoAdmittedUsers « tout le monde »-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="06fa6-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="06fa6-116">Pour plus d’informations, consultez la rubrique [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="06fa6-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
