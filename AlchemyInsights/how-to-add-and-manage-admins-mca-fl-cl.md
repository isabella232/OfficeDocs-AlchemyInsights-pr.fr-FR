---
title: Comment ajouter et gérer des administrateurs
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755437"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="a404a-102">Comment ajouter et gérer des administrateurs</span><span class="sxs-lookup"><span data-stu-id="a404a-102">How to add and manage admins</span></span>

<span data-ttu-id="a404a-103">En fonction de la description de votre problème, nous avons trouvé une solution pour vous.</span><span class="sxs-lookup"><span data-stu-id="a404a-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="a404a-104">La plupart des clients pouvaient résoudre leurs propres problèmes après avoir suivi notre documentation.</span><span class="sxs-lookup"><span data-stu-id="a404a-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="a404a-105">Pour gérer votre compte de facturation pour un accord client Microsoft (MCA), vous pouvez utiliser différents rôles avec le niveau d’accès souhaité.</span><span class="sxs-lookup"><span data-stu-id="a404a-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="a404a-106">Ces rôles s’ajoutent aux rôles de service Azure intégrés qui vous permettent de contrôler vos ressources.</span><span class="sxs-lookup"><span data-stu-id="a404a-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="a404a-107">**Pour ajouter des rôles de facturation dans le portail Azure, procédez comme suit :**</span><span class="sxs-lookup"><span data-stu-id="a404a-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="a404a-108">Connectez-vous au [Portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="a404a-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="a404a-109">Recherchez *gestion des coûts + facturation*.</span><span class="sxs-lookup"><span data-stu-id="a404a-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="a404a-110">Sélectionnez contrôle d’accès (IAM) dans une étendue telle que le compte de facturation, le profil de facturation ou la section facture où vous souhaitez accorder l’accès.</span><span class="sxs-lookup"><span data-stu-id="a404a-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="a404a-111">La page de contrôle d’accès (IAM) répertorie les utilisateurs et les groupes qui sont affectés à chaque rôle pour cette étendue.</span><span class="sxs-lookup"><span data-stu-id="a404a-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="a404a-112">Pour accorder l’accès à un utilisateur, sélectionnez **Ajouter** à partir du haut de la page.</span><span class="sxs-lookup"><span data-stu-id="a404a-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="a404a-113">Dans la liste déroulante *rôle* , sélectionnez un rôle.</span><span class="sxs-lookup"><span data-stu-id="a404a-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="a404a-114">Entrez l’adresse de messagerie de l’utilisateur auquel vous souhaitez accorder l’accès.</span><span class="sxs-lookup"><span data-stu-id="a404a-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="a404a-115">Sélectionnez **Enregistrer** pour affecter le rôle.</span><span class="sxs-lookup"><span data-stu-id="a404a-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="a404a-116">Pour supprimer l’accès d’un utilisateur, sélectionnez l’utilisateur dont vous souhaitez supprimer l’attribution de rôle.</span><span class="sxs-lookup"><span data-stu-id="a404a-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="a404a-117">Sélectionnez **supprimer**.</span><span class="sxs-lookup"><span data-stu-id="a404a-117">Select **Remove**.</span></span>

<span data-ttu-id="a404a-118">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="a404a-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="a404a-119">Définitions des rôles de facturation</span><span class="sxs-lookup"><span data-stu-id="a404a-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="a404a-120">Rôles et tâches des comptes de facturation</span><span class="sxs-lookup"><span data-stu-id="a404a-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="a404a-121">Prise en main de votre compte de facturation MCA</span><span class="sxs-lookup"><span data-stu-id="a404a-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="a404a-122">Vérifier l’accès à un accord client Microsoft</span><span class="sxs-lookup"><span data-stu-id="a404a-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
