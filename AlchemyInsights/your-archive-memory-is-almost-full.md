---
title: Votre boîte aux lettres d’archivage est presque pleine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950507"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="4acc2-102">Votre boîte aux lettres d’archivage est presque pleine</span><span class="sxs-lookup"><span data-stu-id="4acc2-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="4acc2-103">Si l’utilisateur reçoit l’avertissement ; **Votre boîte aux lettres d’archivage est presque pleine** ou vous devez augmenter la taille de sa boîte aux lettres d’archivage, voici quelques conseils :</span><span class="sxs-lookup"><span data-stu-id="4acc2-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="4acc2-104">Si une licence Exchange Online Plan 1 est attribuée à l’utilisateur, mise à niveau vers **Exchange Online Plan 2** pour augmenter la taille de 50 Go à 100 Go.</span><span class="sxs-lookup"><span data-stu-id="4acc2-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="4acc2-105">Si l’utilisateur est déjà affecté à l’un des services suivants : **Exchange Online Plan 2** ou Exchange Online Plan 1 avec un module Archivage Exchange Online, utilisez les étapes ci-dessous pour activer l’archivage à extension automatique :</span><span class="sxs-lookup"><span data-stu-id="4acc2-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="4acc2-106">[Connectez-vous à Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="4acc2-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="4acc2-107">Exécutez l’let de commande suivante pour l’utilisateur :  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="4acc2-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="4acc2-108">Exécutez l’let de commande suivante pour vérifier qu’elle est activée pour l’utilisateur :  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="4acc2-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="4acc2-109">Pour plus d'informations, consultez les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="4acc2-109">For more information see:</span></span>

- [<span data-ttu-id="4acc2-110"> Activer l’archivage illimité - Aide de l’administrateur - Microsoft 365 Compliance | Documents Microsoft</span><span class="sxs-lookup"><span data-stu-id="4acc2-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="4acc2-111">Limites d’Exchange Online : descriptions de service | Documents Microsoft</span><span class="sxs-lookup"><span data-stu-id="4acc2-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="4acc2-112">Mettre à niveau vers une autre plan d'| Documents Microsoft</span><span class="sxs-lookup"><span data-stu-id="4acc2-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

