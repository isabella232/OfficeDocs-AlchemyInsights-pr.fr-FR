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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505684"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="81785-102">Restaurer un groupe Microsoft 365 supprimé</span><span class="sxs-lookup"><span data-stu-id="81785-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="81785-103">Vous pouvez restaurer un groupe Microsoft 365 supprimé ou Microsoft Teams dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="81785-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="81785-104">Pour vous connecter au Centre d’administration Microsoft 365 et lister les groupes et équipes supprimés, allez au Centre d’administration [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="81785-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="81785-105">**Remarque :** Connectez-vous à l’aide du compte attribué à l’administrateur client ou au rôle d’administrateur des groupes.</span><span class="sxs-lookup"><span data-stu-id="81785-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="81785-106">Sélectionnez le groupe Microsoft 365 supprimé/Teams à restaurer, puis cliquez sur **Restaurer le groupe.**</span><span class="sxs-lookup"><span data-stu-id="81785-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="81785-107">Si le groupe ne peut pas être restauré en raison d’une adresse SMTP conflictuelle, utilisez la commande suivante pour rechercher l’objet à l’origine du conflit et supprimez l’adresse SMTP :</span><span class="sxs-lookup"><span data-stu-id="81785-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="81785-108">**Remarque :** Dans certains cas, la restauration du groupe et de toutes ses données peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="81785-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="81785-109">Pour plus d’informations ou pour découvrir comment restaurer des groupes à l’aide de PowerShell, voir Restaurer un groupe [Microsoft 365 supprimé.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="81785-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>