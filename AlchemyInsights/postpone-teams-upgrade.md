---
title: Différer la mise à niveau de Teams
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801229"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="fafbf-102">Comment reporter la mise à niveau de Teams pilotée par Microsoft</span><span class="sxs-lookup"><span data-stu-id="fafbf-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="fafbf-103">**Important**: nous pouvons vous aider à résoudre ce problème à l'aide d'un diagnostic de support, mais il semble que vous n'utilisiez pas le Nouveau Centre d'administration.</span><span class="sxs-lookup"><span data-stu-id="fafbf-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="fafbf-104">Pour utiliser le Nouveau Centre d'administration, faites glisser  le basculement en haut à droite qui indique nouveau centre d'administration à droite.</span><span class="sxs-lookup"><span data-stu-id="fafbf-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="fafbf-105">À l'aide du Nouveau Centre d'administration, cliquez sur le **widget** Besoin d'aide, tapez « Différer la mise à niveau de Teams », puis suivez les invites pour exécuter le diagnostic.</span><span class="sxs-lookup"><span data-stu-id="fafbf-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="fafbf-106">Si vous avez reçu une communication sur une mise à niveau automatisée pilotée par Microsoft de Skype Entreprise vers Microsoft Teams et que vous  souhaitez reporter la mise  à niveau automatisée à une date ultérieure, votre administrateur général peut se connecter au portail d'administration [Teams](https://admin.teams.microsoft.com/dashboard) et, après avoir sélectionné le bouton Actualiser l'état sous Mise à niveau de Microsoft Teams, sélectionnez le bouton Différer.</span><span class="sxs-lookup"><span data-stu-id="fafbf-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="fafbf-107">Pour voir la nouvelle date de la mise à niveau automatisée de votre client vers Microsoft Teams, actualisez la page du portail d'administration teams.</span><span class="sxs-lookup"><span data-stu-id="fafbf-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="fafbf-108">**Remarque :** Le **bouton Différer** sera disponible uniquement si vous avez reçu la notification du centre de messages concernant la mise à niveau automatisée.</span><span class="sxs-lookup"><span data-stu-id="fafbf-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="fafbf-109">Les administrateurs globaux peuvent également [exécuter Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) pour en savoir plus sur leur état actuel de mise à niveau.</span><span class="sxs-lookup"><span data-stu-id="fafbf-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
