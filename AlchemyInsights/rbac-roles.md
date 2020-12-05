---
title: 'Rôles RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576529"
---
# <a name="rbac-rules"></a><span data-ttu-id="2efdc-102">Règles RBAC</span><span class="sxs-lookup"><span data-stu-id="2efdc-102">RBAC rules</span></span>

<span data-ttu-id="2efdc-103">Si vous obtenez l’erreur d’autorisation :</span><span class="sxs-lookup"><span data-stu-id="2efdc-103">If you get the permission error:</span></span> 

- <span data-ttu-id="2efdc-104">**Le client avec l’ID d’objet n’est pas autorisé à effectuer des actions sur l’étendue (code : AuthorizationFailed)**: lorsque vous essayez de créer une ressource, vérifiez que vous êtes actuellement connecté avec un utilisateur auquel est affecté un rôle disposant d’une autorisation en écriture sur la ressource au niveau de l’étendue sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="2efdc-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="2efdc-105">Par exemple, pour gérer des machines virtuelles dans un groupe de ressources, vous devez avoir le rôle de [collaborateur d’ordinateur virtuel](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) sur le groupe de ressources (ou l’étendue parent).</span><span class="sxs-lookup"><span data-stu-id="2efdc-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="2efdc-106">Pour obtenir la liste des autorisations pour chaque rôle intégré, consultez la rubrique [rôles intégrés pour les ressources Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2efdc-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="2efdc-107">**Vous n’êtes pas autorisé à créer une demande de support**: lorsque vous essayez de créer ou de mettre à jour un ticket de support, vérifiez que vous êtes actuellement connecté avec un utilisateur auquel est affecté un rôle qui dispose de l’autorisation Microsoft. support/supportTickets/écriture, comme [support demander le collaborateur](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="2efdc-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="2efdc-108">**Aucune attribution de rôle supplémentaire ne peut être créée (code : RoleAssignmentLimitExceeded)**: lorsque vous essayez d’affecter un rôle, essayez de réduire le nombre d’attributions de rôles en affectant à la place des rôles à des groupes.</span><span class="sxs-lookup"><span data-stu-id="2efdc-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="2efdc-109">Azure prend en charge jusqu’à **2000** attributions de rôles par abonnement.</span><span class="sxs-lookup"><span data-stu-id="2efdc-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="2efdc-110">Pour plus d’informations sur les rôles RBAC Azure, reportez-vous à [Azure RBAC Roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2efdc-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
