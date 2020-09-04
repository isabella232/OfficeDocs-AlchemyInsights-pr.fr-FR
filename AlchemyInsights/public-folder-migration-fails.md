---
title: Échec de la migration de dossiers publics à 95%
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
ms.openlocfilehash: c1c4210baf93f0071a12f1902fb5f6fbf7bd0716
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341384"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="78f1b-102">Échec de la migration de dossiers publics à 95%</span><span class="sxs-lookup"><span data-stu-id="78f1b-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="78f1b-103">Vous avez peut-être initié un lot de migration, et son état continue d’afficher **Synchronisé** pendant une période très longue.</span><span class="sxs-lookup"><span data-stu-id="78f1b-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="78f1b-104">Il s'agit d'un comportement normal.</span><span class="sxs-lookup"><span data-stu-id="78f1b-104">This is expected behavior.</span></span>

<span data-ttu-id="78f1b-105">Il est fréquent que l’état d’un lot de migration reste sur **Synchronisé** pendant quelques heures avant qu’il ne passe à **Finalisation**.</span><span class="sxs-lookup"><span data-stu-id="78f1b-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="78f1b-106">Pour les migrations impliquant un grand nombre de boîtes aux lettres cibles, il est normal de voir l’état Synchronisé pendant plus de 24 heures, pour autant qu’aucune des demandes de migration de dossiers publics sous-jacentes n’ait échoué ou n’ait été mise en quarantaine.</span><span class="sxs-lookup"><span data-stu-id="78f1b-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="78f1b-107">Merci de laisser 24 à 48 heures au lot de migration pour effectuer les tâches.</span><span class="sxs-lookup"><span data-stu-id="78f1b-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="78f1b-108">Pour les migrations de dossier public qui échouent à 95%, avec l’erreur FailedToMailEnablePublicFoldersException :</span><span class="sxs-lookup"><span data-stu-id="78f1b-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="78f1b-109">Téléchargez et exécutez le script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sur votre serveur Exchange local.</span><span class="sxs-lookup"><span data-stu-id="78f1b-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="78f1b-110">Effectuez les actions correctives suggérées par le script.</span><span class="sxs-lookup"><span data-stu-id="78f1b-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="78f1b-111">Exécutez le Sync-MailPublicFolders (pour Exchange 2010) ou Sync-ModernMailPublicFolders (pour Exchange 2013 et versions ultérieures).</span><span class="sxs-lookup"><span data-stu-id="78f1b-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="78f1b-112">Reprendre la migration de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="78f1b-112">Resume public folder migration.</span></span>
