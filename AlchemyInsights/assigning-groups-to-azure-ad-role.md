---
title: Attribution de groupes au rôle Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875365"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="93589-102">Attribution de groupes au rôle Azure AD</span><span class="sxs-lookup"><span data-stu-id="93589-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="93589-103">Pour attribuer un groupe Azure AD ayant la source d’autorité dans Azure AD à un rôle Azure AD, effectuez ces étapes :</span><span class="sxs-lookup"><span data-stu-id="93589-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="93589-104">Créer un groupe : Pour créer un groupe :</span><span class="sxs-lookup"><span data-stu-id="93589-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="93589-105">a.</span><span class="sxs-lookup"><span data-stu-id="93589-105">a.</span></span> <span data-ttu-id="93589-106">Connectez-vous au centre d’administration Azure AD avec des autorisations **d’administrateur de rôle privilégié** ou **d’administrateur général**.</span><span class="sxs-lookup"><span data-stu-id="93589-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="93589-107">b.</span><span class="sxs-lookup"><span data-stu-id="93589-107">b.</span></span> <span data-ttu-id="93589-108">Sélectionnez **Azure Active Directory > Groupes > Tous les groupes > Nouveau groupe**.</span><span class="sxs-lookup"><span data-stu-id="93589-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="93589-109">c.</span><span class="sxs-lookup"><span data-stu-id="93589-109">c.</span></span> <span data-ttu-id="93589-110">Créer le groupe.</span><span class="sxs-lookup"><span data-stu-id="93589-110">Create the group.</span></span>

2. <span data-ttu-id="93589-111">Attribuez le rôle au groupe lors de la création du groupe ou après la création du groupe.</span><span class="sxs-lookup"><span data-stu-id="93589-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="93589-112">a.</span><span class="sxs-lookup"><span data-stu-id="93589-112">a.</span></span> <span data-ttu-id="93589-113">Pour attribuer un rôle au groupe au moment de la création du groupe, basculez sur le bouton bascule **Des rôles Azure AD peuvent être attribués au groupe**, puis créer le groupe.</span><span class="sxs-lookup"><span data-stu-id="93589-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="93589-114">b.</span><span class="sxs-lookup"><span data-stu-id="93589-114">b.</span></span> <span data-ttu-id="93589-115">Pour attribuer un rôle au groupe après sa création, accédez à l’onglet **Rôles attribués** du nouveau groupe, puis attribuez le rôle au groupe.</span><span class="sxs-lookup"><span data-stu-id="93589-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="93589-116">**Gérer l’adhésion à un groupe affecté à un rôle Azure AD**</span><span class="sxs-lookup"><span data-stu-id="93589-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="93589-117">Pour empêcher l’élévation des privilèges, par défaut, seuls les administrateurs de rôles privilégiés et les administrateurs globaux peuvent modifier l’adhésion d’un groupe affecté à un rôle.</span><span class="sxs-lookup"><span data-stu-id="93589-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="93589-118">Toutefois, ils peuvent choisir d’affecter un propriétaire à un tel groupe et déléguer cette tâche.</span><span class="sxs-lookup"><span data-stu-id="93589-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="93589-119">Pour plus de détails sur l’affectation de groupes cloud à des rôles Azure AD, consultez[Attribuer des rôles AD aux groupes cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="93589-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="93589-120">Pour plus détails sur le dépannage des rôles attribués aux groupes cloud, consultez [Résoudre les problèmes liés aux rôles affectés aux groupes cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="93589-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





