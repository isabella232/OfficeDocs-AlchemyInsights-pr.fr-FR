---
title: Vérifier les adresses de forwarding sur les boîtes aux lettres
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403309"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="22643-102">Vérifier les adresses de forwarding sur les boîtes aux lettres</span><span class="sxs-lookup"><span data-stu-id="22643-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="22643-103">Parfois, les pirates informatiques envoient les messages électroniques des utilisateurs à eux-mêmes. Nous allons donc d’abord vérifier les adresses et les règles de forwarding sur la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="22643-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="22643-104">Ensuite, nous vérifierons les journaux d’audit.</span><span class="sxs-lookup"><span data-stu-id="22643-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="22643-105">Voici comment vérifier les adresses de forwarding :</span><span class="sxs-lookup"><span data-stu-id="22643-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="22643-106">Sélectionnez   >  **Utilisateurs actifs.**</span><span class="sxs-lookup"><span data-stu-id="22643-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="22643-107">Sélectionnez l’utilisateur dont le compte a été compromis.</span><span class="sxs-lookup"><span data-stu-id="22643-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="22643-108">Dans le volant qui s’affiche, développez **Paramètres du courrier,** puis cliquez sur **Modifier** pour **le forwarding de courrier électronique.**</span><span class="sxs-lookup"><span data-stu-id="22643-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="22643-109">Supprimez les adresses de forwarding que vous ne connaissez pas.</span><span class="sxs-lookup"><span data-stu-id="22643-109">Remove any forwarding addresses you don't recognize.</span></span>