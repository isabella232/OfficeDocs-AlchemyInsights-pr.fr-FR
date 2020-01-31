---
title: Impossible de supprimer des éléments dans SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571250"
---
# <a name="unable-to-delete-items"></a>Impossible de supprimer les éléments

Les stratégies de rétention peuvent provoquer cela, vous devez désactiver ou exclure le blocage respectif qui est à l’origine du problème. Après la suppression d’une stratégie de rétention ou d’une conservation, la modification peut prendre jusqu’à 24 heures. Assurez-vous qu’il n’y a pas de configuration de [stratégie de rétention](https://docs.microsoft.com/office365/securitycompliance/retention-policies) sur l’élément.

Le site a peut-être dépassé la limite de stockage, augmentez le [quota du site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) et supprimez l’élément.

Vérifiez que l’élément n’est pas [extrait](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) pour un autre utilisateur.

Enfin, les administrateurs peuvent utiliser les [modèles et pratiques SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) qui contiennent une bibliothèque de commandes PowerShell qui vous permettent d’effectuer des actions de gestion complexes, telles que la suppression forcée d’éléments Stubborn.
- [Supprimer le fichier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Supprimer le dossier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Supprimer l’élément de liste PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Supprimer la liste PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Supprimer le champ PNP (colonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)