---
title: Contourner la salle d'entrée
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
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820032"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="01f3c-102">Contrôler les paramètres de salle d'accueil et le niveau de participation dans Teams</span><span class="sxs-lookup"><span data-stu-id="01f3c-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="01f3c-103">Si vous souhaitez autoriser tout le monde, y compris les utilisateurs de connexion, externes et anonymes, à contourner la salle d'entrée, utilisez PowerShell pour accomplir cette tâche.</span><span class="sxs-lookup"><span data-stu-id="01f3c-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="01f3c-104">Voici un exemple de modification de la stratégie de réunion globale pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="01f3c-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="01f3c-105">Cette cmdlet nécessite actuellement l'utilisation du module PowerShell Skype Entreprise.</span><span class="sxs-lookup"><span data-stu-id="01f3c-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="01f3c-106">Pour vous configurer pour utiliser cette cmdlet, consultez La gestion des [stratégies via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="01f3c-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="01f3c-107">Une fois que vous avez installé une stratégie, vous devez l'appliquer aux utilisateurs . ou, si vous avez modifié la stratégie globale, elle s'appliquera automatiquement aux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="01f3c-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="01f3c-108">Pour toute modification de stratégie, vous devez attendre au moins 4 heures **jusqu'à 24** heures pour que les stratégies prennent effet.</span><span class="sxs-lookup"><span data-stu-id="01f3c-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="01f3c-109">Veillez à consulter la documentation ci-dessous avant d'apporter ces modifications pour comprendre exactement ce que cela permet.</span><span class="sxs-lookup"><span data-stu-id="01f3c-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="01f3c-110">Comprendre les contrôles de stratégie de salle d'accueil des réunions Teams</span><span class="sxs-lookup"><span data-stu-id="01f3c-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="01f3c-111">Ces paramètres contrôlent les participants à la réunion qui attendent dans la salle d'attente avant d'être admis à la réunion et le niveau de participation qu'ils sont autorisés à participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="01f3c-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="01f3c-112">Vous pouvez utiliser PowerShell pour mettre à jour les paramètres de stratégie de réunion qui n'ont pas encore été implémentés (étiquetés « bientôt ») dans le Centre d'administration Teams.</span><span class="sxs-lookup"><span data-stu-id="01f3c-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="01f3c-113">Voir ci-dessous un exemple d'cmdlet PowerShell qui permet à tous les utilisateurs de contourner la salle d'entrée.</span><span class="sxs-lookup"><span data-stu-id="01f3c-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="01f3c-114">[Admettre automatiquement les](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) personnes est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d'attente jusqu'à ce qu'elles soient admis par un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="01f3c-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="01f3c-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Autoriser les personnes anonymes à démarrer une réunion est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris les utilisateurs B2B et fédérés, peuvent participer à la réunion de l'utilisateur sans qu'un utilisateur authentifié de l'organisation y participe.</span><span class="sxs-lookup"><span data-stu-id="01f3c-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="01f3c-116">Autoriser les utilisateurs d'appels [rendez-vous](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) à contourner la salle d'attente **(bientôt** disponible) est une stratégie par  organisateur qui contrôle si les personnes qui appellent par téléphone rejoignent la réunion directement ou attendent dans la salle d'attente, quel que soit le paramètre Admettre automatiquement les personnes.</span><span class="sxs-lookup"><span data-stu-id="01f3c-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="01f3c-117">Autoriser les organisateurs à remplacer les [paramètres](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) de la salle d'accueil **(bientôt** disponible) est une stratégie  par organisateur qui contrôle si l'organisateur de la réunion peut remplacer les paramètres de salle d'accueil qu'un administrateur a définies dans Admettre automatiquement les personnes et autoriser les utilisateurs à se rendre à la conférence **rendez-vous** à ignorer la salle d'entrée lorsqu'ils organisent une nouvelle réunion.</span><span class="sxs-lookup"><span data-stu-id="01f3c-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="01f3c-118">**Remarque :** Pour une vue d'ensemble complète des stratégies de réunion Microsoft Teams, voir Gérer les stratégies de réunion dans [Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="01f3c-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
