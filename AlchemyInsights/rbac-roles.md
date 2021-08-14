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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923129"
---
# <a name="rbac-rules"></a>Règles RBAC

Si vous obtenez l’erreur d’autorisation : 

- Le client avec l’ID d’objet n’est pas autorisé à effectuer une action sur l’étendue (code : **AuthorizationFailed)**: lorsque vous essayez de créer une ressource, vérifiez que vous êtes actuellement connecté avec un utilisateur affecté à un rôle qui dispose d’une autorisation d’écriture sur la ressource au niveau de l’étendue sélectionnée. Par exemple, pour gérer des machines virtuelles dans un groupe de ressources, vous devez avoir le rôle Collaborateur de [machine](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) virtuelle sur le groupe de ressources (ou l’étendue parent). Pour obtenir la liste des autorisations pour chaque rôle intégré, voir Rôles intégrés [pour les ressources Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vous n’êtes pas autorisé à créer une demande de support : lorsque vous essayez de créer ou de mettre à jour un ticket de support, vérifiez que vous êtes actuellement en train de vous inscrire avec un utilisateur qui dispose **d’un** rôle qui dispose de l’autorisation Microsoft.Support/supportTickets/write, telle que le collaborateur de demande de [support.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Plus aucune attribution de rôle ne peut être créée **(code : RoleAssignmentLimitExceeded)**: lorsque vous essayez d’attribuer un rôle, essayez de réduire le nombre d’attributions de rôles en attribuant des rôles à des groupes à la place. Azure prend en charge **jusqu’à 2 000 attributions** de rôles par abonnement.

Pour plus d’informations sur les rôles RBAC Azure, voir [Rôles RBAC Azure.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
