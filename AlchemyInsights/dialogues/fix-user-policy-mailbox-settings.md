---
title: Corriger les paramètres de stratégie/boîte aux lettres de l’utilisateur
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568497"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="b5f07-102">Corriger les paramètres de stratégie utilisateur/boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="b5f07-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="b5f07-103">Les paramètres de courrier indésirable de la boîte aux lettres ont affecté ce message.</span><span class="sxs-lookup"><span data-stu-id="b5f07-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="b5f07-104">Pour passer en revue les paramètres, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="b5f07-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="b5f07-105">Lancez l’Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="b5f07-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="b5f07-106">Pour plus d'informations, voir [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="b5f07-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="b5f07-107">Exécutez cette commande (à l’aide de l’adresse e-mail de l’utilisateur)  **: get-mailboxjunkmailconfiguration -identity « user@domain.com »**</span><span class="sxs-lookup"><span data-stu-id="b5f07-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="b5f07-108">Vérifiez si l’adresse e-mail de l’expéditeur fait partie de **TrustedSendersAndDomains** ou **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="b5f07-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="b5f07-109">Si l’adresse de messagerie se trouve dans l’une des listes, vous de devez peut-être la supprimer.</span><span class="sxs-lookup"><span data-stu-id="b5f07-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="b5f07-110">Pour plus d’informations, [voir Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="b5f07-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
