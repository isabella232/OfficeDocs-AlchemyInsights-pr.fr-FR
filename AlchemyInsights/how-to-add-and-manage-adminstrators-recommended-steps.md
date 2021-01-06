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
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="1ae24-102">Procédure d’ajout et de gestion des administrateurs-étapes recommandées</span><span class="sxs-lookup"><span data-stu-id="1ae24-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="1ae24-103">En fonction de la description de votre problème, nous avons trouvé une solution pour vous.</span><span class="sxs-lookup"><span data-stu-id="1ae24-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="1ae24-104">La plupart des clients pouvaient résoudre leurs propres problèmes après avoir suivi notre documentation.</span><span class="sxs-lookup"><span data-stu-id="1ae24-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="1ae24-105">**Modifier l’administrateur de l’abonnement ou le co-administrateur**</span><span class="sxs-lookup"><span data-stu-id="1ae24-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="1ae24-106">L’administrateur de compte peut modifier les deux rôles, tandis que l’administrateur des abonnements peut uniquement modifier les co-administrateurs dans le [portail Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="1ae24-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="1ae24-107">Ajouter ou modifier des administrateurs d’abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="1ae24-108">**Mettre à jour l’administrateur d’abonnement ou Co-Administrator pour les abonnements internes (diffusé)**</span><span class="sxs-lookup"><span data-stu-id="1ae24-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="1ae24-109">L’administrateur de service ou le co-administrateur peut agir en toute autonomie en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="1ae24-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="1ae24-110">Connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) et cliquez sur **gestion des coûts + facturation** dans le volet de gauche.</span><span class="sxs-lookup"><span data-stu-id="1ae24-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="1ae24-111">Cliquez sur la ligne avec votre abonnement.</span><span class="sxs-lookup"><span data-stu-id="1ae24-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="1ae24-112">Cette opération ouvre la vue d’ensemble de votre abonnement.</span><span class="sxs-lookup"><span data-stu-id="1ae24-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="1ae24-113">Dans le panneau **abonnement** , cliquez sur **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="1ae24-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="1ae24-114">Cliquez sur le bouton **admin du service** .</span><span class="sxs-lookup"><span data-stu-id="1ae24-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="1ae24-115">Entrez l’adresse de messagerie de l’utilisateur que vous souhaitez définir en tant qu’administrateur de service, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="1ae24-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="1ae24-116">**Ajouter/modifier/supprimer un co-administrateur**</span><span class="sxs-lookup"><span data-stu-id="1ae24-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="1ae24-117">Connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) en tant qu’administrateur de service.</span><span class="sxs-lookup"><span data-stu-id="1ae24-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="1ae24-118">Ouvrez les [abonnements](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) et sélectionnez un abonnement.</span><span class="sxs-lookup"><span data-stu-id="1ae24-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="1ae24-119">(Les co-administrateurs peuvent uniquement être attribués au niveau de l’abonnement.)</span><span class="sxs-lookup"><span data-stu-id="1ae24-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="1ae24-120">Accédez à **contrôle d’accès (IAM)**  >  **administrateurs classiques**  >  **Add**  >  **Add co-Administrator** pour ouvrir le volet **Ajouter co-admin** (si l’option Ajouter un co-administrateur est désactivée, cela signifie que vous ne disposez pas des autorisations nécessaires).</span><span class="sxs-lookup"><span data-stu-id="1ae24-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="1ae24-121">Sélectionnez l’utilisateur que vous souhaitez ajouter, puis cliquez sur **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="1ae24-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="1ae24-122">**Pour en savoir plus:**</span><span class="sxs-lookup"><span data-stu-id="1ae24-122">**Learn more:**</span></span>
- [<span data-ttu-id="1ae24-123">Ajouter un co-administrateur</span><span class="sxs-lookup"><span data-stu-id="1ae24-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="1ae24-124">Supprimer un co-administrateur</span><span class="sxs-lookup"><span data-stu-id="1ae24-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="1ae24-125">Modifier l’administrateur de service</span><span class="sxs-lookup"><span data-stu-id="1ae24-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="1ae24-126">Afficher l’administrateur de compte</span><span class="sxs-lookup"><span data-stu-id="1ae24-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="1ae24-127">Gérer l’accès à l’aide du RBAC et du portail Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="1ae24-128">**Ajouter/supprimer des utilisateurs à l’aide d’Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="1ae24-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="1ae24-129">Vous pouvez ajouter de nouveaux utilisateurs ou supprimer des utilisateurs existants de votre organisation Azure Active Directory (Azure AD) :</span><span class="sxs-lookup"><span data-stu-id="1ae24-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="1ae24-130">Pour ajouter un nouvel utilisateur, connectez-vous au [portail Azure](https://ms.portal.azure.com/#home) en tant qu’administrateur d’utilisateur de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="1ae24-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="1ae24-131">Sélectionnez **Azure Active Directory**, sélectionnez **utilisateurs** , puis cliquez sur **nouvel utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="1ae24-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="1ae24-132">Sur la page **utilisateur** , remplissez les informations requises.</span><span class="sxs-lookup"><span data-stu-id="1ae24-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="1ae24-133">Cliquez sur **Créer**.</span><span class="sxs-lookup"><span data-stu-id="1ae24-133">Click **Create**.</span></span> <span data-ttu-id="1ae24-134">L’utilisateur est créé et ajouté à votre client Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1ae24-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="1ae24-135">**Pour plus d’informations, voir**:</span><span class="sxs-lookup"><span data-stu-id="1ae24-135">**Learn more**:</span></span>

- [<span data-ttu-id="1ae24-136">Ajouter un nouvel utilisateur</span><span class="sxs-lookup"><span data-stu-id="1ae24-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="1ae24-137">Supprimer un utilisateur</span><span class="sxs-lookup"><span data-stu-id="1ae24-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="1ae24-138">Ajouter ou mettre à jour les informations de profil d’un utilisateur à l’aide d’Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1ae24-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="1ae24-139">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="1ae24-139">**Recommended documents**</span></span>

- [<span data-ttu-id="1ae24-140">Qu’est-ce que le contrôle d’accès basé sur un rôle (RBAC) ?</span><span class="sxs-lookup"><span data-stu-id="1ae24-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="1ae24-141">Comprendre les différents rôles dans Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="1ae24-142">Autorisations des rôles d’administrateur dans Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1ae24-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="1ae24-143">Didacticiel : accorder l’accès d’un utilisateur à l’aide du RBAC et du portail Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="1ae24-144">Résoudre les problèmes liés à RBAC dans Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="1ae24-145">Organiser vos ressources avec des groupes de gestion Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="1ae24-146">Procédure de demande d’une copie de la facture Azure par courrier électronique</span><span class="sxs-lookup"><span data-stu-id="1ae24-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="1ae24-147">Procédure d’ajout, de mise à jour ou de suppression d’une carte bancaire d’Azure</span><span class="sxs-lookup"><span data-stu-id="1ae24-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="1ae24-148">Gérer un abonnement (réactiver/annuler/basculer)</span><span class="sxs-lookup"><span data-stu-id="1ae24-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



