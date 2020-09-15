---
title: Échec de la migration de dossiers publics à 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662421"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="732c6-102">Échec de la migration de dossiers publics à 95%</span><span class="sxs-lookup"><span data-stu-id="732c6-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="732c6-103">Vous avez peut-être initié un lot de migration, et son état continue d’afficher **Synchronisé** pendant une période très longue.</span><span class="sxs-lookup"><span data-stu-id="732c6-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="732c6-104">Il s'agit d'un comportement normal.</span><span class="sxs-lookup"><span data-stu-id="732c6-104">This is expected behavior.</span></span>

<span data-ttu-id="732c6-105">Il est fréquent que l’état d’un lot de migration reste sur **Synchronisé** pendant quelques heures avant qu’il ne passe à **Finalisation**.</span><span class="sxs-lookup"><span data-stu-id="732c6-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="732c6-106">Pour les migrations impliquant un grand nombre de boîtes aux lettres cibles, il est normal de voir l’état Synchronisé pendant plus de 24 heures, pour autant qu’aucune des demandes de migration de dossiers publics sous-jacentes n’ait échoué ou n’ait été mise en quarantaine.</span><span class="sxs-lookup"><span data-stu-id="732c6-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="732c6-107">Merci de laisser 24 à 48 heures au lot de migration pour effectuer les tâches.</span><span class="sxs-lookup"><span data-stu-id="732c6-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="732c6-108">Pour les migrations de dossier public qui échouent à 95%, avec l’erreur FailedToMailEnablePublicFoldersException :</span><span class="sxs-lookup"><span data-stu-id="732c6-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="732c6-109">Téléchargez et exécutez le script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sur votre serveur Exchange local.</span><span class="sxs-lookup"><span data-stu-id="732c6-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="732c6-110">Effectuez les actions correctives suggérées par le script.</span><span class="sxs-lookup"><span data-stu-id="732c6-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="732c6-111">Exécutez le Sync-MailPublicFolders (pour Exchange 2010) ou Sync-ModernMailPublicFolders (pour Exchange 2013 et versions ultérieures).</span><span class="sxs-lookup"><span data-stu-id="732c6-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="732c6-112">Reprendre la migration de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="732c6-112">Resume public folder migration.</span></span>
