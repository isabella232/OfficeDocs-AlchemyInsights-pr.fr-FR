---
title: Différer la mise à niveau des équipes
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741769"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="e1548-102">Ajournement de la mise à niveau des équipes basées sur Microsoft</span><span class="sxs-lookup"><span data-stu-id="e1548-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="e1548-103">**Important**: nous pouvons vous aider à résoudre ce problème pour vous en utilisant un diagnostic du support technique, mais il semble que vous n’utilisiez pas le nouveau centre d’administration.</span><span class="sxs-lookup"><span data-stu-id="e1548-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="e1548-104">Pour utiliser le nouveau centre d’administration, faites glisser le bouton bascule en haut à droite qui indique **nouveau centre d’administration** à droite.</span><span class="sxs-lookup"><span data-stu-id="e1548-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="e1548-105">À l’aide du nouveau centre d’administration, cliquez sur le widget **besoin d’aide ?** , tapez « différer la mise à niveau des équipes », puis suivez les invites pour exécuter le diagnostic.</span><span class="sxs-lookup"><span data-stu-id="e1548-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="e1548-106">Si vous avez reçu une communication sur une mise à niveau automatisée basée sur Microsoft de Skype entreprise vers Microsoft teams et que vous souhaitez reporter la mise à niveau automatique à une date ultérieure, votre administrateur général peut se connecter au [portail d’administration de teams](https://admin.teams.microsoft.com/dashboard) et, après avoir sélectionné le bouton **Actualiser** dans la section mise à niveau de Microsoft Teams, sélectionnez le bouton **reporter** .</span><span class="sxs-lookup"><span data-stu-id="e1548-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="e1548-107">Pour afficher la nouvelle date de mise à niveau automatisée de votre client vers Microsoft Teams, actualisez la page du portail d’administration de teams.</span><span class="sxs-lookup"><span data-stu-id="e1548-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="e1548-108">**Remarque :** Le bouton **reporter** n’est disponible que si vous avez reçu la notification du centre de messages concernant la mise à niveau automatisée.</span><span class="sxs-lookup"><span data-stu-id="e1548-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="e1548-109">Les administrateurs globaux peuvent également exécuter [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) pour en savoir plus sur l’état actuel de la mise à niveau.</span><span class="sxs-lookup"><span data-stu-id="e1548-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
