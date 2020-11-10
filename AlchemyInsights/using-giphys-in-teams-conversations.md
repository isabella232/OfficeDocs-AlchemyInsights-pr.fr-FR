---
title: Utilisation de images giphy dans les conversations de teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947491"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="0cdb2-102">Utilisation de images giphy dans les conversations de teams</span><span class="sxs-lookup"><span data-stu-id="0cdb2-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="0cdb2-103">L’accès images giphy dans Team Chat est activé par défaut.</span><span class="sxs-lookup"><span data-stu-id="0cdb2-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="0cdb2-104">En tant qu’administrateur, vous pouvez contrôler si images giphy est disponible pour les utilisateurs en [définissant une stratégie de messagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) et en vous assurant que **l’utilisation de images giphy dans les conversations** est **activée**.</span><span class="sxs-lookup"><span data-stu-id="0cdb2-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="0cdb2-105">Si les images gif ne fonctionnent pas comme prévu dans les conversations de teams, vérifiez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="0cdb2-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="0cdb2-106">La [stratégie de messagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) doit autoriser images giphy.</span><span class="sxs-lookup"><span data-stu-id="0cdb2-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="0cdb2-107">Pour vérifier à l’aide des cmdlets PowerShell, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="0cdb2-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="0cdb2-108">Vérifiez que vous pouvez [gérer teams avec PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="0cdb2-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="0cdb2-109">Exécutez la commande PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) et vérifiez que **AllowGiphy** est défini sur **true**.</span><span class="sxs-lookup"><span data-stu-id="0cdb2-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="0cdb2-110">Si **AllowGiphy** est défini sur **false** , exécutez la commande PowerShell suivante [Set-CsTeamsMessagingPolicy-identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="0cdb2-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="0cdb2-111">Les [expériences en connexion facultatives](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) doivent être activées pour permettre l’accès à l’URL Giphy.</span><span class="sxs-lookup"><span data-stu-id="0cdb2-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="0cdb2-112">Si plusieurs stratégies de messagerie de teams sont configurées pour votre client, vous pouvez déterminer l’identité de la stratégie attribuée à l’utilisateur concerné à l’aide de la commande PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Sélectionnez TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="0cdb2-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
