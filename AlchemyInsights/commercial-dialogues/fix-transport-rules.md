---
title: Corriger les règles de transport
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737133"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="046a0-102">Corriger les règles de transport</span><span class="sxs-lookup"><span data-stu-id="046a0-102">Fix transport rules</span></span>

<span data-ttu-id="046a0-103">Une règle de flux de messagerie personnalisée a affecté ce message.</span><span class="sxs-lookup"><span data-stu-id="046a0-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="046a0-104">Pour passer en revue la règle exacte, faites les choses suivantes :</span><span class="sxs-lookup"><span data-stu-id="046a0-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="046a0-105">Dans les résultats de la soumission, sous **Informations supplémentaires,** notez le **GUID** ou le nom **de la stratégie.**</span><span class="sxs-lookup"><span data-stu-id="046a0-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="046a0-106">Lancez l’Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="046a0-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="046a0-107">Pour plus d'informations, voir [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="046a0-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="046a0-108">Exécutez cette commande (à l’aide du GUID de votre soumission) :  **Get-TransportRule -identity « GUID » | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="046a0-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="046a0-109">Consultez la description pour voir les conditions configurées qui ont affecté le message.</span><span class="sxs-lookup"><span data-stu-id="046a0-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="046a0-110">Pour plus d’informations, [voir Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="046a0-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
