---
title: Rôle de gestion des identités privilégiées
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086284"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="ba0be-102">Rôle de gestion des identités avec privilèges (PIM)</span><span class="sxs-lookup"><span data-stu-id="ba0be-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="ba0be-103">**Les autorisations ne sont pas accordées après l’activation d’un rôle**</span><span class="sxs-lookup"><span data-stu-id="ba0be-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="ba0be-104">Lorsque vous activez un rôle dans Azure AD Privileged Identity Management (PIM), l’activation peut ne pas se propager instantanément à tous les portails qui nécessitent le rôle privilégié.</span><span class="sxs-lookup"><span data-stu-id="ba0be-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="ba0be-105">Parfois, même si la modification est propagée, la mise en cache Web dans un portail peut empêcher le changement de prendre effet immédiatement.</span><span class="sxs-lookup"><span data-stu-id="ba0be-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="ba0be-106">Si votre activation est retardée, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ba0be-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="ba0be-107">Déconnectez-vous du portail Azure, puis reconnectez-vous.</span><span class="sxs-lookup"><span data-stu-id="ba0be-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="ba0be-108">Lorsque vous activez un rôle Azure AD ou un rôle de ressource Azure, vous verrez les étapes de votre activation.</span><span class="sxs-lookup"><span data-stu-id="ba0be-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="ba0be-109">Une fois toutes les étapes terminées, vous verrez un lien « Déconnexion ».</span><span class="sxs-lookup"><span data-stu-id="ba0be-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="ba0be-110">Vous pouvez utiliser ce lien pour vous déconnecter. Cela permet de résoudre la plupart des cas de retard d’activation.</span><span class="sxs-lookup"><span data-stu-id="ba0be-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="ba0be-111">Dans le GIP, vérifiez que vous êtes répertorié en tant que membre du rôle.</span><span class="sxs-lookup"><span data-stu-id="ba0be-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="ba0be-112">Si vous activez le rôle Administrateur Exchange, assurez-vous de vous déconnecter et de vous reconnecter.</span><span class="sxs-lookup"><span data-stu-id="ba0be-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="ba0be-113">Si le problème persiste, ouvrez un ticket de support et signalez-le comme un problème.</span><span class="sxs-lookup"><span data-stu-id="ba0be-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="ba0be-114">Si vous utilisez votre rôle d’administrateur Exchange pour accéder au centre de sécurité et de conformité, reportez-vous à l’étape suivante.</span><span class="sxs-lookup"><span data-stu-id="ba0be-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="ba0be-115">Si vous activez un rôle pour accéder au centre de sécurité et de conformité ou si vous activez le rôle d’administrateur SharePoint, vous constaterez un certain délai d’activation de quelques minutes à quelques heures.</span><span class="sxs-lookup"><span data-stu-id="ba0be-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="ba0be-116">Il s’agit d’un problème connu que nous collaborons activement avec ces équipes pour résoudre ce problème dès que possible.</span><span class="sxs-lookup"><span data-stu-id="ba0be-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="ba0be-117">Pour plus d’informations, reportez-vous aux rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="ba0be-117">For more information, see:</span></span>

- [<span data-ttu-id="ba0be-118">Activer mes rôles Azure AD dans PIM</span><span class="sxs-lookup"><span data-stu-id="ba0be-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="ba0be-119">Activer mes rôles de ressource Azure dans PIM</span><span class="sxs-lookup"><span data-stu-id="ba0be-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="ba0be-120">**Les autorisations ne sont pas supprimées après la désactivation d’un rôle ou l’activation de rôle expire**</span><span class="sxs-lookup"><span data-stu-id="ba0be-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="ba0be-121">Lorsque vous désactivez un rôle dans Azure AD Privileged Identity Management ou lorsqu’une période d’activation de rôle arrive à expiration, il se peut que vous continuiez à avoir accès.</span><span class="sxs-lookup"><span data-stu-id="ba0be-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="ba0be-122">Si votre désactivation est retardée, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ba0be-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="ba0be-123">Si vous désactivez le rôle d’administrateur Exchange ou que la période d’activation de rôle expire, et que vous remarquez un retard important avant la suppression des autorisations, ouvrez un ticket de support et indiquez à votre ingénieur de support de classer un ticket avec l’équipe PAM (Privileged Access Management) dans Office à propos de ce problème.</span><span class="sxs-lookup"><span data-stu-id="ba0be-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="ba0be-124">Si la période d’activation a expiré, mais que vous avez toujours ouvert la session de navigateur, fermez votre navigateur.</span><span class="sxs-lookup"><span data-stu-id="ba0be-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="ba0be-125">Vous pouvez continuer à utiliser le rôle jusqu’à ce que vous fermiez cette session.</span><span class="sxs-lookup"><span data-stu-id="ba0be-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="ba0be-126">Il s’agit d’un problème connu et nous examinons un correctif potentiel pour révoquer activement chaque session une fois l’activation expirée.</span><span class="sxs-lookup"><span data-stu-id="ba0be-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="ba0be-127">Si votre retard diffère de celui de ces deux scénarios, veuillez ouvrir un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="ba0be-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
