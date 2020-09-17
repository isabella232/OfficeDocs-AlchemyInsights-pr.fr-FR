---
title: Blocage du téléchargement via des liens de partage
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685740"
---
# <a name="block-download-on-sharing-links"></a>Blocage du téléchargement via des liens de partage

**Bloquer le téléchargement** est disponible pour les **liens en affichage seul** vers les documents Office. Lorsque vous sélectionnez cette option, les personnes qui accèdent au fichier via le lien que vous avez créé ne voient pas les options de téléchargement, d’impression ni de copie du fichier.

Les administrateurs peuvent contrôler si le paramètre Bloquer le téléchargement s’affiche uniquement pour les fichiers Office ou non en modifiant le paramètre de `BlockDownloadLinksFileType` dans les cmdlets PowerShell [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) ou [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps).
