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
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903550"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="ffc18-102">Échec de la migration de dossiers publics à 95%</span><span class="sxs-lookup"><span data-stu-id="ffc18-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="ffc18-103">Pour les migrations de dossier public qui échouent à 95%, avec l’erreur FailedToMailEnablePublicFoldersException :</span><span class="sxs-lookup"><span data-stu-id="ffc18-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="ffc18-104">Téléchargez et exécutez le script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sur votre serveur Exchange local.</span><span class="sxs-lookup"><span data-stu-id="ffc18-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="ffc18-105">Effectuez les actions correctives suggérées par le script.</span><span class="sxs-lookup"><span data-stu-id="ffc18-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="ffc18-106">Exécutez le Sync-MailPublicFolders (pour Exchange 2010) ou Sync-ModernMailPublicFolders (pour Exchange 2013 et versions ultérieures).</span><span class="sxs-lookup"><span data-stu-id="ffc18-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="ffc18-107">Reprendre la migration de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="ffc18-107">Resume public folder migration.</span></span>
