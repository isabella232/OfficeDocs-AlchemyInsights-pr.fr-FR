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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806109"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="da7df-102">Impossible de supprimer les éléments</span><span class="sxs-lookup"><span data-stu-id="da7df-102">Unable to delete items</span></span>

<span data-ttu-id="da7df-103">Les stratégies de rétention peuvent provoquer cela, vous devez désactiver ou exclure le blocage respectif qui est à l’origine du problème.</span><span class="sxs-lookup"><span data-stu-id="da7df-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="da7df-104">Après la suppression d’une stratégie de rétention ou d’une conservation, la modification peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="da7df-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="da7df-105">Assurez-vous qu’il n’y a pas de configuration de [stratégie de rétention](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="da7df-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="da7df-106">Le site a peut-être dépassé la limite de stockage, augmentez le [quota du site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) et supprimez l’élément.</span><span class="sxs-lookup"><span data-stu-id="da7df-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="da7df-107">Vérifiez que l’élément n’est pas [extrait](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) pour un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="da7df-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="da7df-108">Enfin, les administrateurs peuvent utiliser les [modèles et pratiques SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) qui contiennent une bibliothèque de commandes PowerShell qui vous permettent d’effectuer des actions de gestion complexes, telles que la suppression forcée d’éléments Stubborn.</span><span class="sxs-lookup"><span data-stu-id="da7df-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="da7df-109">Supprimer le fichier PNP</span><span class="sxs-lookup"><span data-stu-id="da7df-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="da7df-110">Supprimer le dossier PNP</span><span class="sxs-lookup"><span data-stu-id="da7df-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="da7df-111">Supprimer l’élément de liste PNP</span><span class="sxs-lookup"><span data-stu-id="da7df-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="da7df-112">Supprimer la liste PNP</span><span class="sxs-lookup"><span data-stu-id="da7df-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="da7df-113">Supprimer le champ PNP (colonne)</span><span class="sxs-lookup"><span data-stu-id="da7df-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)