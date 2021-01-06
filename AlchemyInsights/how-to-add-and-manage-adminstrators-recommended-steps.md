---
title: Procédure d’ajout et de gestion des administrateurs-étapes recommandées
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755833"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Procédure d’ajout et de gestion des administrateurs-étapes recommandées

En fonction de la description de votre problème, nous avons trouvé une solution pour vous. La plupart des clients pouvaient résoudre leurs propres problèmes après avoir suivi notre documentation.

**Modifier l’administrateur de l’abonnement ou le co-administrateur**

- L’administrateur de compte peut modifier les deux rôles, tandis que l’administrateur des abonnements peut uniquement modifier les co-administrateurs dans le [portail Azure](https://ms.portal.azure.com/#home).
- [Ajouter ou modifier des administrateurs d’abonnements Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Mettre à jour l’administrateur d’abonnement ou Co-Administrator pour les abonnements internes (diffusé)**

L’administrateur de service ou le co-administrateur peut agir en toute autonomie en procédant comme suit :

1. Connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) et cliquez sur **gestion des coûts + facturation** dans le volet de gauche.
2. Cliquez sur la ligne avec votre abonnement. Cette opération ouvre la vue d’ensemble de votre abonnement.
3. Dans le panneau **abonnement** , cliquez sur **Propriétés**. 
4. Cliquez sur le bouton **admin du service** .
5. Entrez l’adresse de messagerie de l’utilisateur que vous souhaitez définir en tant qu’administrateur de service, puis cliquez sur **OK**.

**Ajouter/modifier/supprimer un co-administrateur**

1. Connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) en tant qu’administrateur de service.
2. Ouvrez les [abonnements](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) et sélectionnez un abonnement. (Les co-administrateurs peuvent uniquement être attribués au niveau de l’abonnement.)
3. Accédez à **contrôle d’accès (IAM)**  >  **administrateurs classiques**  >  **Add**  >  **Add co-Administrator** pour ouvrir le volet **Ajouter co-admin** (si l’option Ajouter un co-administrateur est désactivée, cela signifie que vous ne disposez pas des autorisations nécessaires).
4. Sélectionnez l’utilisateur que vous souhaitez ajouter, puis cliquez sur **Ajouter**.

**Pour en savoir plus:**
- [Ajouter un co-administrateur](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Supprimer un co-administrateur](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Modifier l’administrateur de service](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Afficher l’administrateur de compte](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gérer l’accès à l’aide du RBAC et du portail Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Ajouter/supprimer des utilisateurs à l’aide d’Azure Active Directory (AD)**

Vous pouvez ajouter de nouveaux utilisateurs ou supprimer des utilisateurs existants de votre organisation Azure Active Directory (Azure AD) :

1. Pour ajouter un nouvel utilisateur, connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) en tant qu’administrateur d’utilisateur de l’organisation.
2. Sélectionnez **Azure Active Directory**, sélectionnez **utilisateurs** , puis cliquez sur **nouvel utilisateur**.
3. Sur la page **utilisateur** , remplissez les informations requises. Cliquez sur **Créer**. L’utilisateur est créé et ajouté à votre client Azure AD.

**Pour plus d’informations, voir**:

- [Ajouter un nouvel utilisateur](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Supprimer un utilisateur](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Ajouter ou mettre à jour les informations de profil d’un utilisateur à l’aide d’Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documents recommandés**

- [Qu’est-ce que le contrôle d’accès basé sur un rôle (RBAC) ?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Comprendre les différents rôles dans Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Autorisations des rôles d’administrateur dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Didacticiel : accorder l’accès d’un utilisateur à l’aide du RBAC et du portail Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Résoudre les problèmes liés à RBAC dans Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organiser vos ressources avec des groupes de gestion Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Procédure de demande d’une copie de la facture Azure par courrier électronique](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Procédure d’ajout, de mise à jour ou de suppression d’une carte bancaire d’Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gérer un abonnement (réactiver/annuler/basculer)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



