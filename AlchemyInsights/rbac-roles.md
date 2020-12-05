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
# <a name="rbac-rules"></a>Règles RBAC

Si vous obtenez l’erreur d’autorisation : 

- **Le client avec l’ID d’objet n’est pas autorisé à effectuer des actions sur l’étendue (code : AuthorizationFailed)**: lorsque vous essayez de créer une ressource, vérifiez que vous êtes actuellement connecté avec un utilisateur auquel est affecté un rôle disposant d’une autorisation en écriture sur la ressource au niveau de l’étendue sélectionnée. Par exemple, pour gérer des machines virtuelles dans un groupe de ressources, vous devez avoir le rôle de [collaborateur d’ordinateur virtuel](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) sur le groupe de ressources (ou l’étendue parent). Pour obtenir la liste des autorisations pour chaque rôle intégré, consultez la rubrique [rôles intégrés pour les ressources Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Vous n’êtes pas autorisé à créer une demande de support**: lorsque vous essayez de créer ou de mettre à jour un ticket de support, vérifiez que vous êtes actuellement connecté avec un utilisateur auquel est affecté un rôle qui dispose de l’autorisation Microsoft. support/supportTickets/écriture, comme [support demander le collaborateur](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Aucune attribution de rôle supplémentaire ne peut être créée (code : RoleAssignmentLimitExceeded)**: lorsque vous essayez d’affecter un rôle, essayez de réduire le nombre d’attributions de rôles en affectant à la place des rôles à des groupes. Azure prend en charge jusqu’à **2000** attributions de rôles par abonnement.

Pour plus d’informations sur les rôles RBAC Azure, reportez-vous à [Azure RBAC Roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
