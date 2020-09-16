---
title: L’expéditeur ne reçoit pas le courrier envoyé au groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751313"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="8f651-102">L’expéditeur ne reçoit pas le courrier envoyé au groupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8f651-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="8f651-103">Par défaut, l’expéditeur d’un message électronique envoyé à un groupe Microsoft 365 ne reçoit pas de copie du message dans sa boîte de réception, même s’il est membre du groupe.</span><span class="sxs-lookup"><span data-stu-id="8f651-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="8f651-104">Utilisez cette commande PowerShell EXO pour autoriser l’expéditeur à recevoir une copie de chaque message qu’il envoie au groupe Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="8f651-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="8f651-105">Pour activer le paramètre pour toutes les boîtes aux lettres à la fois :</span><span class="sxs-lookup"><span data-stu-id="8f651-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="8f651-106">**Remarque** Une heure peut s’écouler avant que les modifications apportées à ce paramètre prennent effet.</span><span class="sxs-lookup"><span data-stu-id="8f651-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>