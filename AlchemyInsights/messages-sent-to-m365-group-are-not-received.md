---
title: Les messages envoyés au groupe Microsoft 365 ne sont pas reçus par tous les membres
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823785"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="e25f5-102">Les messages envoyés à un groupe Microsoft 365 ne sont pas reçus par tous les membres</span><span class="sxs-lookup"><span data-stu-id="e25f5-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="e25f5-103">Veuillez à ce que tous les membres du groupe soient abonnés pour recevoir les e-mails.</span><span class="sxs-lookup"><span data-stu-id="e25f5-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="e25f5-104">Voir [Suivre un groupe dans Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="e25f5-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="e25f5-105">Pour vérifier l’état des messages des membres qui se sont abonnés aux e-mails de groupe, exécutez la commande suivante sur [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) :</span><span class="sxs-lookup"><span data-stu-id="e25f5-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="e25f5-106">Utilisez la commande PowerShell EXO pour configurer tous les membres du groupe de manière à ce qu’ils reçoivent les messages envoyés à un groupe Microsoft 365 dans leur boîte de réception :</span><span class="sxs-lookup"><span data-stu-id="e25f5-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="e25f5-107">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="e25f5-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`