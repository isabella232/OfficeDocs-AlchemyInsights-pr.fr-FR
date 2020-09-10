---
title: Le lot de migration de dossiers publics n’aboutit pas et la mention « Synchronisé » apparaît
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406560"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="3e606-102">Le lot de migration de dossiers publics n’aboutit pas et la mention « Synchronisé » apparaît</span><span class="sxs-lookup"><span data-stu-id="3e606-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="3e606-103">Vous avez peut-être initié un lot de migration, et l’état de cette migration affiche « Synchronisé » sur une très longue période.</span><span class="sxs-lookup"><span data-stu-id="3e606-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="3e606-104">Il s'agit d'un comportement normal.</span><span class="sxs-lookup"><span data-stu-id="3e606-104">This is expected behavior.</span></span>

<span data-ttu-id="3e606-105">Il est fréquent que l’état d’un lot de migration reste sur « Synchronisé » pendant quelques heures avant qu’il ne passe à « Finalisation ».</span><span class="sxs-lookup"><span data-stu-id="3e606-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="3e606-106">Pour les migrations impliquant un grand nombre de boîtes aux lettres cibles, il est normal que l’état affiche « Synchronisé » pendant plus de 24 heures, pour autant qu’aucune des demandes de migration de dossiers publics sous-jacentes n’ait échoué ou n’ait été mise en quarantaine.</span><span class="sxs-lookup"><span data-stu-id="3e606-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="3e606-107">Il convient de laisser 24 à 48 heures au lot de migration pour effectuer les tâches.</span><span class="sxs-lookup"><span data-stu-id="3e606-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
