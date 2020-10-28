---
title: Accès aux abonnements
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773773"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="959b1-102">Impossible de se connecter à Azure en raison de problèmes de navigateur (blocage du navigateur, continuité de l’exécution, pas chargement, etc.)</span><span class="sxs-lookup"><span data-stu-id="959b1-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="959b1-103">Vous pouvez être concerné par une panne.</span><span class="sxs-lookup"><span data-stu-id="959b1-103">You might be impacted by an outage.</span></span> <span data-ttu-id="959b1-104">Vérifiez s’il existe une panne en cours : état d' [intégrité Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="959b1-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="959b1-105">Déconnectez-vous de toutes les sessions Azure actives.</span><span class="sxs-lookup"><span data-stu-id="959b1-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="959b1-106">Démarrez un mode Incognito ou de votre navigateur Web.</span><span class="sxs-lookup"><span data-stu-id="959b1-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="959b1-107">Vous pouvez également essayer d’actualiser le navigateur, d’utiliser un autre navigateur, de supprimer les cookies de cache si vous ne travaillez pas.</span><span class="sxs-lookup"><span data-stu-id="959b1-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="959b1-108">En savoir plus : [résoudre les problèmes de connexion](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="959b1-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="959b1-109">**Impossible d’accéder aux abonnements**</span><span class="sxs-lookup"><span data-stu-id="959b1-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="959b1-110">Dans le [portail Azure](https://portal.azure.com/), assurez-vous que le répertoire Azure approprié est sélectionné à partir du compte dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="959b1-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="959b1-111">Dans le [Centre de comptes Azure](https://account.windowsazure.com/Subscriptions), assurez-vous que le compte utilisé est l’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="959b1-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="959b1-112">En savoir plus : [dépanner aucun abonnement trouvé](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="959b1-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="959b1-113">**Impossible d’accéder à l’historique de facturation**</span><span class="sxs-lookup"><span data-stu-id="959b1-113">**Unable to access billing history**</span></span>

<span data-ttu-id="959b1-114">L’administrateur de compte doit s’assurer que l’utilisateur qui accède aux informations de facturation est ajouté à Azure Active Directory en tant qu’utilisateur invité : [Ajouter ou supprimer un nouvel utilisateur](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="959b1-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="959b1-115">L’utilisateur doit ensuite disposer d’un rôle d’administrateur global : [attribuer un rôle aux utilisateurs](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="959b1-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="959b1-116">Publier ce message, l’utilisateur peut bénéficier d’un accès de facturation à l’aide de stratégies RBAC : [accorder l’accès à la facturation](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="959b1-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="959b1-117">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="959b1-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="959b1-118">Je ne parviens pas à me connecter pour gérer mon abonnement Azure</span><span class="sxs-lookup"><span data-stu-id="959b1-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)