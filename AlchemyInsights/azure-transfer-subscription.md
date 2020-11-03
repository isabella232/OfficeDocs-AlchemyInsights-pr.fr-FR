---
title: Transférer la propriété de facturation Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840606"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="ef8b0-102">Transférer la propriété de facturation Azure</span><span class="sxs-lookup"><span data-stu-id="ef8b0-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="ef8b0-103">Connectez-vous au [portail Azure](https://portal.azure.com/) comme administrateur du compte de facturation qui contient l’abonnement que vous voulez transférer.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="ef8b0-104">Si vous ne savez pas si vous êtes administrateur, ou si vous avez besoin de déterminer qui l’est, voir [Déterminer l’administrateur de facturation d’un compte](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="ef8b0-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="ef8b0-105">Recherchez sur **Gestion des coûts + Facturation**.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="ef8b0-106">Sélectionnez **Abonnements** dans le volet gauche.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="ef8b0-107">Selon l’accès, vous devrez peut-être sélectionner une étendue de facturation, puis **Abonnements** ou **Abonnements Azure**.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="ef8b0-108">Sélectionnez **Transférer la propriété de facturation** pour l’abonnement que vous voulez transférer.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="ef8b0-109">Entrez l’adresse e-mail d’un utilisateur qui est un administrateur de facturation du compte qui sera le nouveau propriétaire de l’abonnement, puis sélectionnez **envoyer une demande de transfert**</span><span class="sxs-lookup"><span data-stu-id="ef8b0-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="ef8b0-110">L’utilisateur reçoit un e-mail contenant des instructions pour examiner votre demande de transfert.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="ef8b0-111">Pour approuver la demande de transfert, l’utilisateur sélectionne le lien dans l’email et suit les instructions.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="ef8b0-112">**Remarque**  : si vous transférez la propriété de facturation à un compte d’utilisateur dans un autre client Azure AD, toutes les attributions de [contrôle d’accès en fonction du rôle (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) servant à gérer les ressources dans l’abonnement sont supprimées définitivement.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="ef8b0-113">Seul le nouveau propriétaire peut accéder à la gestion des ressources dans l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ef8b0-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="ef8b0-114">Pour plus d’informations, consultez [transfert d’un abonnement à un utilisateur dans un autre client Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ef8b0-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ef8b0-115">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="ef8b0-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="ef8b0-116">Transférer la propriété de facturation d’un abonnement Azure vers un autre compte</span><span class="sxs-lookup"><span data-stu-id="ef8b0-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="ef8b0-117">À propos du transfert de propriété de facturation pour un abonnement Azure</span><span class="sxs-lookup"><span data-stu-id="ef8b0-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="ef8b0-118">Transfert des abonnements Visual Studio, Microsoft Partner Network (MPN) et Dev/Test avec paiement à l’utilisation</span><span class="sxs-lookup"><span data-stu-id="ef8b0-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="ef8b0-119">FAQ Transfert de propriété</span><span class="sxs-lookup"><span data-stu-id="ef8b0-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="ef8b0-120">Résoudre les problèmes de transfert de propriété</span><span class="sxs-lookup"><span data-stu-id="ef8b0-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
