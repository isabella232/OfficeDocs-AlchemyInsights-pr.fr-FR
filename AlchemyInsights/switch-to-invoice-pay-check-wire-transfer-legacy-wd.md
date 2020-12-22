---
title: Basculer vers le paiement de facture (chèque/virement bancaire)-WD héritée
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
- "9004168"
- "7343"
ms.openlocfilehash: 1be90771f994e832960383b1cb5e0bee8f5b08f8
ms.sourcegitcommit: b561c339926fad609950ac92744c3cd91e0a68fa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49722821"
---
# <a name="switch-to-invoice-pay-chequewire-transfer---legacy-wd"></a><span data-ttu-id="c8357-102">Basculer vers le paiement de facture (chèque/virement bancaire)-WD héritée</span><span class="sxs-lookup"><span data-stu-id="c8357-102">Switch to invoice pay (cheque/wire transfer) - Legacy WD</span></span>

<span data-ttu-id="c8357-103">Si vous passez en mode paiement par facture, cela signifie que vous payez votre facture dans les 30 jours suivant la date de facturation.</span><span class="sxs-lookup"><span data-stu-id="c8357-103">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="c8357-104">Pour pouvoir payer votre abonnement Azure par facture, soumettez une demande au support Azure.</span><span class="sxs-lookup"><span data-stu-id="c8357-104">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="c8357-105">Une fois que votre demande est approuvée, vous pouvez passer un abonnement au paiement de facture dans le [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c8357-105">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="c8357-106">**Avant de poursuivre, consultez les conditions requises/limitations suivantes lors de la demande de l’option de paiement de facture :**</span><span class="sxs-lookup"><span data-stu-id="c8357-106">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="c8357-107">Connectez-vous au [portail Azure](https://portal.azure.com/) et accédez à modes de paiement.</span><span class="sxs-lookup"><span data-stu-id="c8357-107">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="c8357-108">Vérifiez que vous êtes déjà approuvé pour le paiement de la facture.</span><span class="sxs-lookup"><span data-stu-id="c8357-108">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="c8357-109">Le paiement de facture est uniquement disponible pour les comptes professionnels, pas pour les comptes personnels.</span><span class="sxs-lookup"><span data-stu-id="c8357-109">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="c8357-110">Vous devez payer tous les frais impayés avant de passer au paiement de facture.</span><span class="sxs-lookup"><span data-stu-id="c8357-110">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="c8357-111">L’équipe de support technique examinera le compte pour déterminer s’il est éligible au mode de paiement de la facture.</span><span class="sxs-lookup"><span data-stu-id="c8357-111">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="c8357-112">Le mode de paiement de la facture n’est pas pris en charge pour les services tiers de marché ; Si vous avez l’intention de basculer un abonnement actuel vers une facture qui contient des services Marketplace ou tiers, ces services doivent être supprimés avant le basculement.</span><span class="sxs-lookup"><span data-stu-id="c8357-112">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="c8357-113">Pour les futures services de marché, achetez d’abord un abonnement distinct sur la carte de crédit, puis achetez ou déployez des services tiers.</span><span class="sxs-lookup"><span data-stu-id="c8357-113">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="c8357-114">Une fois que vous avez basculé vers le paiement de facture, vous ne pouvez plus revenir au paiement par carte bancaire.</span><span class="sxs-lookup"><span data-stu-id="c8357-114">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="c8357-115">*Une fois que vous êtes autorisé à payer par facture*, vous pouvez faire en sorte que votre abonnement Azure à la facture soit payé via chèque ou transfert bancaire dans le  [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c8357-115">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="c8357-116">Pour cela :</span><span class="sxs-lookup"><span data-stu-id="c8357-116">To do that:</span></span>

1. <span data-ttu-id="c8357-117">Connectez-vous au [portail Azure](https://portal.azure.com/)   en tant qu’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="c8357-117">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="c8357-118">Recherchez et sélectionnez **gestion des coûts + facturation**.</span><span class="sxs-lookup"><span data-stu-id="c8357-118">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="c8357-119">Sélectionnez l’abonnement que vous souhaitez passer au paiement de la facture.</span><span class="sxs-lookup"><span data-stu-id="c8357-119">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="c8357-120">Sélectionnez **modes de paiement**.</span><span class="sxs-lookup"><span data-stu-id="c8357-120">Select **Payment methods**.</span></span>
3. <span data-ttu-id="c8357-121">Dans la barre de commandes, cliquez sur le bouton **payer par facture** .</span><span class="sxs-lookup"><span data-stu-id="c8357-121">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="c8357-122">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="c8357-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="c8357-123">Demande/téléchargement/affichage de votre facture Azure facturation et des données d’utilisation</span><span class="sxs-lookup"><span data-stu-id="c8357-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="c8357-124">Comment envoyer des courriers électroniques Azure directement à votre boîte de réception</span><span class="sxs-lookup"><span data-stu-id="c8357-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="c8357-125">Payer par facture</span><span class="sxs-lookup"><span data-stu-id="c8357-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="c8357-126">Comprendre les frais d’utilisation détaillés</span><span class="sxs-lookup"><span data-stu-id="c8357-126">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="c8357-127">Comprendre les termes de votre facture</span><span class="sxs-lookup"><span data-stu-id="c8357-127">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="c8357-128">Comment transférer la propriété</span><span class="sxs-lookup"><span data-stu-id="c8357-128">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
