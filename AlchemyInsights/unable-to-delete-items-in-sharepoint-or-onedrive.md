---
title: Impossible de supprimer des éléments dans SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057708"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="5a563-102">Impossible de supprimer les éléments</span><span class="sxs-lookup"><span data-stu-id="5a563-102">Unable to delete items</span></span>

<span data-ttu-id="5a563-103">Vous rencontrez des problèmes lors de la suppression d’éléments?</span><span class="sxs-lookup"><span data-stu-id="5a563-103">Having issues deleting items?</span></span>

- <span data-ttu-id="5a563-104">Vérifiez toujours que vous disposez des [autorisations appropriées](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) pour supprimer l’élément ou que l' [administrateur](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) de la collection de sites tente de supprimer l’élément.</span><span class="sxs-lookup"><span data-stu-id="5a563-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="5a563-105">Assurez-vous qu’il n’y a pas de configuration de [stratégie](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) de rétention sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="5a563-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="5a563-106">Vérifiez que l’élément n’est pas [extrait](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) pour un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5a563-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="5a563-107">Enfin, les administrateurs peuvent utiliser les [modèles et pratiques SharePoint](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) qui contiennent une bibliothèque de commandes PowerShell qui vous permettent d’effectuer des actions de gestion complexes, telles que la suppression forcée d’éléments Stubborn.</span><span class="sxs-lookup"><span data-stu-id="5a563-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="5a563-108">Supprimer le fichier PNP</span><span class="sxs-lookup"><span data-stu-id="5a563-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="5a563-109">Supprimer le dossier PNP</span><span class="sxs-lookup"><span data-stu-id="5a563-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="5a563-110">Supprimer l’élément de liste PNP</span><span class="sxs-lookup"><span data-stu-id="5a563-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="5a563-111">Supprimer la liste PNP</span><span class="sxs-lookup"><span data-stu-id="5a563-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="5a563-112">Supprimer le champ PNP (colonne)</span><span class="sxs-lookup"><span data-stu-id="5a563-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)