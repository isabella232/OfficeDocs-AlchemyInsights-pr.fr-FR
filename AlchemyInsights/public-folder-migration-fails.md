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
# <a name="public-folder-migration-fails-at-95"></a>Échec de la migration de dossiers publics à 95%

Pour les migrations de dossier public qui échouent à 95%, avec l’erreur FailedToMailEnablePublicFoldersException :

1. Téléchargez et exécutez le script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sur votre serveur Exchange local.

2. Effectuez les actions correctives suggérées par le script.

3. Exécutez le Sync-MailPublicFolders (pour Exchange 2010) ou Sync-ModernMailPublicFolders (pour Exchange 2013 et versions ultérieures).

4. Reprendre la migration de dossiers publics.
