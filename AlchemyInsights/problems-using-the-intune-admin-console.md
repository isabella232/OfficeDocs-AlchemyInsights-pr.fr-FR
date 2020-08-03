---
title: Problèmes liés à l’utilisation de la console d’administration Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46523016"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="06c76-102">Problèmes liés à l’utilisation de la console d’administration Intune</span><span class="sxs-lookup"><span data-stu-id="06c76-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="06c76-103">**« Accès refusé » lors de la navigation dans le portail d’administration Intune.**</span><span class="sxs-lookup"><span data-stu-id="06c76-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="06c76-104">Si vous êtes membre d’un rôle personnalisé Intune, vérifiez qu’une licence Intune ou Enterprise Mobility Suite (EMS) est attribuée à votre compte.</span><span class="sxs-lookup"><span data-stu-id="06c76-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="06c76-105">Si vous utilisez Configuration Manager pour gérer les appareils, vérifiez que vous ne faites pas partie de la collection d’utilisateurs Intune pour Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="06c76-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="06c76-106">Vérifiez que les autorisations de contrôle d’administration basée sur les rôles (RBAC) appropriées vous sont attribuées dans le panneau de rôles Intune.</span><span class="sxs-lookup"><span data-stu-id="06c76-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="06c76-107">Vérifiez que le groupe utilisé n’est pas une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="06c76-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="06c76-108">Intune dans le portail Microsoft Azure prend uniquement en charge les comptes d’utilisateur appartenant aux groupes de sécurité Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="06c76-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="06c76-109">Vérifiez vos groupes sur le portail Microsoft Azure > **Intune** > **Groupes**, ou sur le portail Microsoft Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="06c76-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="06c76-110">**L’utilisateur a trop d’autorisations pour le rôle Intune attribué**</span><span class="sxs-lookup"><span data-stu-id="06c76-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="06c76-111">Invitez l’utilisateur à accéder à **Intune** > **Rôles Intune** > **Mes autorisations** > **Exporter** pour vérifier les autorisations accordées.</span><span class="sxs-lookup"><span data-stu-id="06c76-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="06c76-112">**J’ai ajouté un groupe d’étendues à un rôle, mais les utilisateurs de ce rôle voient toujours les autres utilisateurs ou appareils.**</span><span class="sxs-lookup"><span data-stu-id="06c76-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="06c76-113">Les groupes d’étendues ne filtrent pas les utilisateurs ou les appareils.</span><span class="sxs-lookup"><span data-stu-id="06c76-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="06c76-114">Groupes d’étendues :</span><span class="sxs-lookup"><span data-stu-id="06c76-114">Scope groups:</span></span>

- <span data-ttu-id="06c76-115">Limiter les utilisateurs auxquels vous pouvez attribuer les stratégies ou applications.</span><span class="sxs-lookup"><span data-stu-id="06c76-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="06c76-116">Autoriser uniquement des utilisateurs spécifiques à exécuter des tâches distantes sur des appareils.</span><span class="sxs-lookup"><span data-stu-id="06c76-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="06c76-117">Si vous souhaitez obtenir davantage d’informations sur les groupes d’étendues, voir [Contrôle d’accès en fonction du rôle (RBAC) avec Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="06c76-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="06c76-118">**J’ai ajouté un utilisateur à un rôle Intune, mais il dispose toujours d’un accès complet à la console d’administration Intune.**</span><span class="sxs-lookup"><span data-stu-id="06c76-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="06c76-119">Accédez à Intune > **Utilisateurs** sur le portail Microsoft Azure et vérifiez que l’un des rôles suivants n’est pas attribué à l’utilisateur sur le portail Microsoft Azure :</span><span class="sxs-lookup"><span data-stu-id="06c76-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="06c76-120">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="06c76-120">Global administrator</span></span>
- <span data-ttu-id="06c76-121">Administrateur du service Intune</span><span class="sxs-lookup"><span data-stu-id="06c76-121">Intune service administrator</span></span>
- <span data-ttu-id="06c76-122">Administrateur SharePoint</span><span class="sxs-lookup"><span data-stu-id="06c76-122">SharePoint administrator</span></span>

<span data-ttu-id="06c76-123">Si vous souhaitez obtenir plus d’informations, consultez la page [Contrôle d’accès en fonction du rôle (RBAC) avec Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="06c76-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="06c76-124">**Problèmes d’accès**</span><span class="sxs-lookup"><span data-stu-id="06c76-124">**Access Issues**</span></span>

<span data-ttu-id="06c76-125">Si vous souhaitez obtenir davantage d’informations, consultez la page [Vous ne pouvez pas vous connecter à Office 365, Azure ou Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="06c76-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>