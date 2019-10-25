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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654254"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="a2438-102">Paramètres de la salle d’attente de contrôle et niveau de participation</span><span class="sxs-lookup"><span data-stu-id="a2438-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="a2438-103">Si vous souhaitez autoriser tout le monde, y compris les utilisateurs d’appels entrants, externes et anonymes à contourner la salle d’attente, vous pouvez utiliser PowerShell pour le faire.</span><span class="sxs-lookup"><span data-stu-id="a2438-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="a2438-104">Voici un exemple de modification de la stratégie de réunion globale pour votre organisation :</span><span class="sxs-lookup"><span data-stu-id="a2438-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="a2438-105">Cette applet de commande requiert actuellement l’utilisation du module Skype entreprise PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a2438-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="a2438-106">Pour obtenir le programme d’installation de cette cmdlet, consultez la rubrique [gestion des stratégies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="a2438-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="a2438-107">Vous pouvez configurer une nouvelle stratégie, que vous devrez ensuite appliquer à vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="a2438-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="a2438-108">Si vous modifiez la stratégie globale, elle s’applique automatiquement aux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="a2438-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="a2438-109">Pour toute modification de stratégie, vous devez attendre au moins 4 heures et jusqu’à 24 heures pour que les stratégies prennent effet.</span><span class="sxs-lookup"><span data-stu-id="a2438-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="a2438-110">Veillez à consulter la documentation ci-dessous avant de faire en sorte que ces modifications comprennent exactement ce que cela autorise.</span><span class="sxs-lookup"><span data-stu-id="a2438-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="a2438-111">Présentation des contrôles de stratégie de salle d’attente de réunion teams</span><span class="sxs-lookup"><span data-stu-id="a2438-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="a2438-112">L' [admission automatique des personnes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) est une stratégie par organisateur qui contrôle si les personnes rejoignent une réunion directement ou attendent dans la salle d’attente jusqu’à ce qu’elles soient admises par un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="a2438-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="a2438-113">[Autoriser les utilisateurs anonymes à démarrer une réunion](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) est une stratégie par organisateur qui contrôle si les personnes anonymes, y compris B2B et les utilisateurs fédérés, peuvent rejoindre la réunion sans utilisateur authentifié de l’organisation en participation.</span><span class="sxs-lookup"><span data-stu-id="a2438-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="a2438-114">Autoriser les utilisateurs de rendez [-vous à contourner le lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si les personnes qui se connectent par téléphone rejoignent la réunion directement ou attendent dans la salle d’attente indépendamment du paramètre **autoriser les personnes automatiquement** .</span><span class="sxs-lookup"><span data-stu-id="a2438-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="a2438-115">[Permettre aux organisateurs de remplacer les paramètres de la salle d’attente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (bientôt**disponible**) est une stratégie par organisateur qui contrôle si l’organisateur de la réunion peut remplacer les paramètres de la salle d’attente qu’un administrateur a défini de manière à **admettre automatiquement les personnes** et **à autoriser les appels entrants utilisateurs à contourner la salle d’attente** lorsqu’ils planifient une nouvelle réunion.</span><span class="sxs-lookup"><span data-stu-id="a2438-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="a2438-116">**Remarque :** Consultez [gérer les stratégies de réunion dans teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pour obtenir une vue d’ensemble des stratégies de réunion Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a2438-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
