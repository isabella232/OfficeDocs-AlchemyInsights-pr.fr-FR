---
title: Empêcher le déplacement automatique des messages vers l’archive
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736940"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="c8065-102">Empêcher le déplacement automatique des messages vers l’archive</span><span class="sxs-lookup"><span data-stu-id="c8065-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="c8065-103">Si vous utilisez une stratégie de rétention, vous pouvez modifier l’âge de rétention dans cette stratégie pour arrêter automatiquement l’archivage des messages.</span><span class="sxs-lookup"><span data-stu-id="c8065-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="c8065-104">Voici comment procéder :</span><span class="sxs-lookup"><span data-stu-id="c8065-104">Here's how:</span></span>

1. <span data-ttu-id="c8065-105">Dans le Centre [d’administration Exchange,](https://go.microsoft.com/fwlink/?linkid=2059104)choisissez les **balises de rétention de gestion** de la  >  **conformité.**</span><span class="sxs-lookup"><span data-stu-id="c8065-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="c8065-106">Recherchez votre balise de rétention Déplacer vers l’archive.</span><span class="sxs-lookup"><span data-stu-id="c8065-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="c8065-107">Dans la balise de rétention, modifiez  la période de rétention (période d’archivage) pour ne jamais empêcher les éléments d’être automatiquement archivés par une stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="c8065-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="c8065-108">Cela modifie le paramètre d’archivage de toutes les boîtes aux lettres avec cette balise de rétention qui leur est appliquée.</span><span class="sxs-lookup"><span data-stu-id="c8065-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
