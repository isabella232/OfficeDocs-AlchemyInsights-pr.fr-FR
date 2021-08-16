---
title: Impossible de supprimer des éléments dans SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038515"
---
# <a name="unable-to-delete-items"></a>Impossible de supprimer des éléments

- Les stratégies de rétention peuvent être à l’origine de ce problème. Vous devez désactiver ou exclure la conservation respective à l’origine de ce problème. Après la suppression d’une stratégie ou d’une conservation de rétention, l’application de la modification peut prendre jusqu’à 24 heures. Assurez-vous qu’il n’existe pas de configuration [de stratégie de](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) rétention sur l’élément.

- Le site peut avoir dépassé la limite de stockage, augmenter le [quota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) et supprimer l’élément.

- Assurez-vous que l’élément [n’est pas extrait par](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) un autre utilisateur.

- Enfin, les administrateurs peuvent utiliser [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), qui contient une bibliothèque de commandes PowerShell qui vous permettent d’effectuer des actions de gestion complexes, telles que la suppression de force de la suppression des éléments d’archive.
- [Supprimer un fichier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Supprimer le dossier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Supprimer un élément de liste PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Supprimer la liste PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Supprimer le champ PNP (colonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)