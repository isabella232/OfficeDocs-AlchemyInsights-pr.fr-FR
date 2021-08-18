---
title: 'Procédure d’ajout et de gestion des administrateurs : étapes recommandées'
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
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339030"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Procédure d’ajout et de gestion des administrateurs : étapes recommandées

En fonction de la description de votre problème, nous avons trouvé une solution pour vous. La plupart des clients ont pu résoudre eux-mêmes leur problème après avoir suivi notre documentation.

**Modifier l’administrateur d’abonnement ou le co-administrateur**

- L’administrateur de compte peut modifier les deux rôles alors que l’administrateur d’abonnement ne peut modifier que les co-administrateurs dans [le portail Azure.](https://ms.portal.azure.com/#home)
- [Ajouter ou modifier des administrateurs d’abonnement Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Mettre à jour l’administrateur dCo-Administrator abonnement pour les abonnements internes (AIRS)**

L’administrateur de service ou le co-administrateur peut auto-servir cette action en suivant les étapes suivantes :

1. Connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) et cliquez sur Gestion des coûts **+ Facturation** dans le bouton gauche.
2. Cliquez sur l’élément de ligne avec votre abonnement. La vue d’ensemble de votre abonnement s’ouvre.
3. Dans le bouton **Abonnement,** cliquez sur **Propriétés.** 
4. Cliquez sur le **bouton Administrateur de** service.
5. Entrez le courrier électronique de l’utilisateur que vous souhaitez définir en tant qu’administrateur de service, puis cliquez sur **OK.**

**Ajouter/modifier/supprimer un co-administrateur**

1. Connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) en tant qu’administrateur de service.
2. Ouvrez [Abonnements](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) et sélectionnez un abonnement. (Les co-administrateurs ne peuvent être affectés qu’au niveau de l’étendue de l’abonnement.)
3. Accédez à Contrôle d’accès **(IAM)** Administrateurs classiques Ajouter un co-administrateur pour ouvrir le volet Ajouter un  >    >    >   co-administrateur (si l’option Ajouter un **co-administrateur** est désactivée, elle indique que vous n’avez pas d’autorisations).
4. Sélectionnez l’utilisateur à ajouter, puis cliquez sur **Ajouter.**

**Pour en savoir plus:**
- [Ajouter un co-administrateur](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Supprimer un co-administrateur](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Modifier l’administrateur de service](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Afficher l’administrateur de compte](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gérer l’accès à l’aide de RBAC et du portail Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Ajouter/supprimer des utilisateurs à l’Azure Active Directory (AD)**

Vous pouvez ajouter de nouveaux utilisateurs ou supprimer des utilisateurs existants de votre organisation Azure Active Directory (Azure AD) :

1. Pour ajouter un nouvel utilisateur, connectez-vous au portail [Azure](https://ms.portal.azure.com/#home) en tant qu’administrateur utilisateur de l’organisation.
2. Sélectionnez **Azure Active Directory,** **sélectionnez Utilisateurs,** puis cliquez **sur Nouvel utilisateur.**
3. Dans la page **Utilisateur,** remplissez les informations requises. Cliquez sur **Créer**. L’utilisateur est créé et ajouté à votre client Azure AD.

**En savoir plus**:

- [Ajouter un nouvel utilisateur](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Supprimer un utilisateur](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Ajouter ou mettre à jour les informations de profil d’un utilisateur à l’aide Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documents recommandés**

- [Qu’est-ce que le contrôle d’accès basé sur un rôle (RBAC) ?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Comprendre les différents rôles dans Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Autorisations des rôles d’administrateur dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Didacticiel : Accorder l’accès à un utilisateur utilisant RBAC et le portail Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Résoudre les problèmes de RBAC dans Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organiser vos ressources avec des groupes de gestion Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Comment demander une copie de la facture Azure par courrier électronique](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Comment ajouter, mettre à jour ou supprimer une carte de crédit ou de débit d’Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gérer (Réactiver/Annuler/Basculer) abonnement](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



