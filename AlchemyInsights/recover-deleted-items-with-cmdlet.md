---
title: Récupérer les objets supprimés avec cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835809"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="06c48-102">Récupérer les objets supprimés avec cmdlet</span><span class="sxs-lookup"><span data-stu-id="06c48-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="06c48-103">Utilisez le [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) pour afficher les éléments supprimés dans les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="06c48-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="06c48-104">Une fois que vous avez trouvé les éléments supprimés, vous utilisez le cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) pour les restaurer.</span><span class="sxs-lookup"><span data-stu-id="06c48-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="06c48-105">Voir tous les détails dans [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="06c48-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="06c48-106">Vous avez besoin d'être assigné au rôle d'importateur-exportateur de boîtes aux lettres avant de pouvoir exécuter ce cmdlet.</span><span class="sxs-lookup"><span data-stu-id="06c48-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="06c48-107">Veuillez voir [la rubrique Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) pour plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="06c48-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
