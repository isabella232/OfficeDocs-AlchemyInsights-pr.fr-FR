---
title: Activer la gestion des coûts
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599061"
---
# <a name="enable-cost-management"></a><span data-ttu-id="31bbc-102">Activer la gestion des coûts</span><span class="sxs-lookup"><span data-stu-id="31bbc-102">Enable cost management</span></span>

<span data-ttu-id="31bbc-103">**Que signifie « les coûts sont désactivés pour votre organisation » ?**</span><span class="sxs-lookup"><span data-stu-id="31bbc-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="31bbc-104">Les organisations qui utilisent des comptes accord entreprise (EA) ou Microsoft client Agreement (MCA) peuvent désactiver l’accès aux informations de coûts et aux informations de tarification.</span><span class="sxs-lookup"><span data-stu-id="31bbc-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="31bbc-105">Une fois connecté au portail Azure, il peut utiliser les API de facturation pour obtenir des factures (par programme) et des détails sur l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="31bbc-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="31bbc-106">**Procédure autoriser les utilisateurs supplémentaires à accéder aux factures**</span><span class="sxs-lookup"><span data-stu-id="31bbc-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="31bbc-107">Accédez à **Blade d’abonnements** dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="31bbc-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="31bbc-108">Sélectionnez **factures** , puis **accès aux factures**.</span><span class="sxs-lookup"><span data-stu-id="31bbc-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="31bbc-109">Activez l’accès, suivi de l’enregistrement des modifications, pour permettre aux utilisateurs de rôles d’étendue d’abonnement de télécharger des factures.</span><span class="sxs-lookup"><span data-stu-id="31bbc-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="31bbc-110">L’administrateur de compte peut également configurer de façon à ce que les factures soient envoyées par courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="31bbc-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="31bbc-111">Pour en savoir plus, consultez [la rubrique obtenir votre facture dans un courrier électronique](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="31bbc-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="31bbc-112">**Comment ajouter des utilisateurs au rôle de lecteur de facturation**</span><span class="sxs-lookup"><span data-stu-id="31bbc-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="31bbc-113">Accédez à **Blade d’abonnements** dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="31bbc-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="31bbc-114">Sélectionnez **contrôle d’accès (IAM)** , puis cliquez sur **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="31bbc-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="31bbc-115">Sélectionnez **lecteur de facturation** dans la page **Sélectionner un rôle** .</span><span class="sxs-lookup"><span data-stu-id="31bbc-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="31bbc-116">Tapez l’adresse de messagerie de l’utilisateur que vous souhaitez inviter, puis cliquez sur **OK** pour envoyer l’invitation.</span><span class="sxs-lookup"><span data-stu-id="31bbc-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="31bbc-117">Suivez les instructions fournies dans le message d’invitation pour vous connecter en tant que lecteur de facturation.</span><span class="sxs-lookup"><span data-stu-id="31bbc-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="31bbc-118">Pour plus d’informations, consultez la rubrique [accorder l’accès à la facturation](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="31bbc-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="31bbc-119">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="31bbc-119">**Recommended documents**</span></span>

- [<span data-ttu-id="31bbc-120">Activer les affichages DA et AO via le portail EA</span><span class="sxs-lookup"><span data-stu-id="31bbc-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="31bbc-121">Coûts inclus dans la gestion des coûts</span><span class="sxs-lookup"><span data-stu-id="31bbc-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="31bbc-122">Offres Microsoft Azure prises en charge</span><span class="sxs-lookup"><span data-stu-id="31bbc-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="31bbc-123">Examiner les coûts dans l’analyse des coûts</span><span class="sxs-lookup"><span data-stu-id="31bbc-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="31bbc-124">Donner accès aux informations de facturation</span><span class="sxs-lookup"><span data-stu-id="31bbc-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="31bbc-125">Vérifier l’accès à un accord client Microsoft</span><span class="sxs-lookup"><span data-stu-id="31bbc-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






