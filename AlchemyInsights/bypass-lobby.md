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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="c166a-102">Contrôler les paramètres de la salle d’attente et le niveau de participation dans teams</span><span class="sxs-lookup"><span data-stu-id="c166a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="c166a-103">Si vous souhaitez autoriser tout le monde, y compris les utilisateurs d’appels entrants, externes et anonymes, à **contourner la salle d’attente**, utilisez PowerShell pour accomplir cette tâche.</span><span class="sxs-lookup"><span data-stu-id="c166a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="c166a-104">Voici un exemple de modification de la stratégie de réunion globale pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c166a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="c166a-105">Cette applet de commande requiert actuellement l’utilisation du module Skype entreprise PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c166a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="c166a-106">Pour configurer l’utilisation de cette cmdlet, consultez la rubrique [gestion des stratégies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="c166a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="c166a-107">Une fois que vous avez configuré une stratégie, vous devez l’appliquer aux utilisateurs ; ou, si vous avez modifié la stratégie globale, elle s’applique automatiquement aux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="c166a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="c166a-108">Pour toute modification de stratégie, vous devez attendre au moins **4 heures jusqu’à 24 heures** pour que les stratégies prennent effet.</span><span class="sxs-lookup"><span data-stu-id="c166a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="c166a-109">Veillez à consulter la documentation ci-dessous avant de faire en sorte que ces modifications comprennent exactement ce que cela autorise.</span><span class="sxs-lookup"><span data-stu-id="c166a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="c166a-110">Présentation des contrôles de stratégie de salle d’attente de réunion teams</span><span class="sxs-lookup"><span data-stu-id="c166a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="c166a-111">Ces paramètres contrôlent les participants à la réunion qui attendent dans la salle d’attente avant d’être admis à la réunion et le niveau de participation qu’ils sont autorisés à participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="c166a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="c166a-112">Vous pouvez utiliser PowerShell pour mettre à jour les paramètres de stratégie de réunion qui n’ont pas encore été mis en œuvre (étiqueté « bientôt disponible ») dans le centre d’administration Teams.</span><span class="sxs-lookup"><span data-stu-id="c166a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="c166a-113">Voir ci-dessous un exemple d’applet de commande PowerShell qui permet à tous les utilisateurs de contourner la salle d’attente.</span><span class="sxs-lookup"><span data-stu-id="c166a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="c166a-114">L' [admission automatique des personnes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admises par un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="c166a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c166a-115">[Autoriser les utilisateurs anonymes à démarrer une réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris B2B et les utilisateurs fédérés, peuvent rejoindre la réunion sans utilisateur authentifié de l’organisation en participation.</span><span class="sxs-lookup"><span data-stu-id="c166a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c166a-116">Autoriser les utilisateurs de rendez [-vous à contourner le lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si les personnes qui se connectent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente indépendamment du paramètre **autoriser les personnes automatiquement** .</span><span class="sxs-lookup"><span data-stu-id="c166a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c166a-117">[Permettre aux organisateurs de remplacer les paramètres de la salle d’attente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de la salle d’attente qu’un administrateur a défini de manière à **admettre automatiquement les personnes** et permettre aux utilisateurs de rendez **-vous de contourner la salle d’attente** lorsqu’ils planifient une nouvelle réunion.</span><span class="sxs-lookup"><span data-stu-id="c166a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c166a-118">**Remarque :** Consultez [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pour obtenir une vue d’ensemble des stratégies de réunion Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c166a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
