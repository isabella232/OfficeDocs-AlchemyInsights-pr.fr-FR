---
title: Restaurer un groupe Microsoft 365 supprimé
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645129"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="229c0-102">Restaurer un groupe Microsoft 365 supprimé</span><span class="sxs-lookup"><span data-stu-id="229c0-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="229c0-103">Vous pouvez restaurer un groupe Microsoft 365 supprimé ou Microsoft Teams dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="229c0-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="229c0-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of you’re the deleted groups and teams.</span><span class="sxs-lookup"><span data-stu-id="229c0-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="229c0-105">**Remarque :** Connectez-vous à l’aide du compte attribué à l’administrateur client ou au rôle d’administrateur des groupes.</span><span class="sxs-lookup"><span data-stu-id="229c0-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="229c0-106">Sélectionnez le groupe Microsoft 365 supprimé/Teams à restaurer, puis cliquez sur **Restaurer le groupe.**</span><span class="sxs-lookup"><span data-stu-id="229c0-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="229c0-107">Si le groupe ne peut pas être restauré en raison d’une adresse SMTP conflictuelle, utilisez la commande suivante pour rechercher l’objet à l’origine du conflit et supprimez l’adresse SMTP :</span><span class="sxs-lookup"><span data-stu-id="229c0-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="229c0-108">**Remarque :** Dans certains cas, la restauration du groupe et de toutes ses données peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="229c0-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="229c0-109">Pour plus d’informations ou pour découvrir comment restaurer des groupes à l’aide de PowerShell, voir Restaurer un groupe [Microsoft 365 supprimé.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="229c0-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>