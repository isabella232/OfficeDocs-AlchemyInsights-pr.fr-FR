---
title: Envoyer en tant que groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740149"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="df3cb-102">Envoyer en tant que groupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="df3cb-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="df3cb-103">Vous pouvez attribuer des autorisations Envoyer en tant que pour permettre à des utilisateurs spécifiques d’envoyer des messages en tant que groupe Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="df3cb-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="df3cb-104">Connectez-vous à Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="df3cb-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="df3cb-105">Exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="df3cb-105">Run the following command:</span></span>  

    <span data-ttu-id="df3cb-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -Trustee AccessRights</span><span class="sxs-lookup"><span data-stu-id="df3cb-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="df3cb-107">Si vous souhaitez obtenir plus d’informations, voir [Autoriser les membres à envoyer en tant que ou de la part d'un groupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="df3cb-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>