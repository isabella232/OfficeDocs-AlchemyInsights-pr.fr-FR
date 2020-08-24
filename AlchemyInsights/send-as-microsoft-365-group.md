---
title: Envoyer en tant que groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46852997"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="ff86f-102">Envoyer en tant que groupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ff86f-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="ff86f-103">Vous pouvez attribuer des autorisations Envoyer en tant que pour permettre à des utilisateurs spécifiques d’envoyer des messages en tant que groupe Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="ff86f-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="ff86f-104">Connectez-vous à Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ff86f-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="ff86f-105">Exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="ff86f-105">Run the following command:</span></span>  

    <span data-ttu-id="ff86f-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -Trustee AccessRights</span><span class="sxs-lookup"><span data-stu-id="ff86f-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="ff86f-107">Si vous souhaitez obtenir plus d’informations, voir [Autoriser les membres à envoyer en tant que ou de la part d'un groupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ff86f-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>