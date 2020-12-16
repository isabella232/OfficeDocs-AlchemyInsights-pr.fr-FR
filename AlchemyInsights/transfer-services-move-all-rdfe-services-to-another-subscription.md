---
title: 'Transfer Services : déplacer tous les services RDFE vers un autre abonnement'
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681461"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="b5a30-102">Transfer Services : déplacer tous les services RDFE vers un autre abonnement</span><span class="sxs-lookup"><span data-stu-id="b5a30-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="b5a30-103">**Déplacer des ressources**</span><span class="sxs-lookup"><span data-stu-id="b5a30-103">**Move resources**</span></span>

<span data-ttu-id="b5a30-104">Les ressources Azure peuvent être déplacées vers un autre abonnement ou groupe de ressources Azure sous le même abonnement à l’aide du portail Azure, d’Azure PowerShell, de l’interface CLI Azure ou de l’API REST pour déplacer des ressources.</span><span class="sxs-lookup"><span data-stu-id="b5a30-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="b5a30-105">Avant de pouvoir déplacer des ressources, voir :</span><span class="sxs-lookup"><span data-stu-id="b5a30-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="b5a30-106">Liste de vérification avant de transférer des ressources</span><span class="sxs-lookup"><span data-stu-id="b5a30-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="b5a30-107">Services pouvant être déplacés</span><span class="sxs-lookup"><span data-stu-id="b5a30-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="b5a30-108">Comment valider le déplacement</span><span class="sxs-lookup"><span data-stu-id="b5a30-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="b5a30-109">Conseils de déplacement pour les services</span><span class="sxs-lookup"><span data-stu-id="b5a30-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="b5a30-110">Pour déplacer des ressources existantes vers un autre groupe de ressources ou abonnement, vous pouvez utiliser les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="b5a30-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="b5a30-111">Portail Azure</span><span class="sxs-lookup"><span data-stu-id="b5a30-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="b5a30-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b5a30-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="b5a30-113">Interface de commande de commande Azure</span><span class="sxs-lookup"><span data-stu-id="b5a30-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="b5a30-114">API REST</span><span class="sxs-lookup"><span data-stu-id="b5a30-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="b5a30-115">Didacticiel : [déplacer des ressources Azure vers un autre groupe de ressources ou abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="b5a30-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="b5a30-116">**Résoudre les erreurs avec Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="b5a30-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="b5a30-117">Consultez les articles ci-dessous pour en savoir plus sur les erreurs de déploiement Azure courantes et recevoir des informations pour les résoudre.</span><span class="sxs-lookup"><span data-stu-id="b5a30-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="b5a30-118">Si vous ne trouvez pas le code d’erreur de votre erreur de déploiement, reportez-vous à la rubrique [Rechercher le code d’erreur](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="b5a30-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="b5a30-119">Résoudre les erreurs de déploiement</span><span class="sxs-lookup"><span data-stu-id="b5a30-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="b5a30-120">Résoudre les problèmes de transfert de ressources Azure vers un nouveau groupe de ressources ou un nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="b5a30-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="b5a30-121">Notez que si vous souhaitez mettre à niveau votre abonnement Azure, par exemple pour passer de la version gratuite à payer en tant que vous-même, vous devrez convertir votre abonnement.</span><span class="sxs-lookup"><span data-stu-id="b5a30-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="b5a30-122">Pour mettre à niveau une version d’évaluation gratuite, consultez [la rubrique mise à niveau de votre version d’évaluation gratuite ou de votre abonnement Microsoft imagine Azure pour payer en tant que vous-même](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="b5a30-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="b5a30-123">Pour modifier un compte facturé en tant que, consultez [la rubrique change your Azure pay-as-do-on-by Subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="b5a30-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="b5a30-124">**Pour ajouter ou associer un abonnement Azure à votre client Azure Active Directory :**</span><span class="sxs-lookup"><span data-stu-id="b5a30-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="b5a30-125">Connectez-vous et sélectionnez l’abonnement que vous souhaitez utiliser à partir de la [page abonnements dans le portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="b5a30-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="b5a30-126">Sélectionnez **changer de répertoire**.</span><span class="sxs-lookup"><span data-stu-id="b5a30-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="b5a30-127">Examinez les avertissements qui s’affichent, puis sélectionnez **modifier**.</span><span class="sxs-lookup"><span data-stu-id="b5a30-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="b5a30-128">Le répertoire est modifié pour l’abonnement et vous obtiendrez un message de réussite.</span><span class="sxs-lookup"><span data-stu-id="b5a30-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="b5a30-129">Utilisez le sélecteur d' *Annuaire* pour accéder à votre nouveau répertoire.</span><span class="sxs-lookup"><span data-stu-id="b5a30-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="b5a30-130">L’affichage correct de tous les éléments peut prendre jusqu’à 10 minutes.</span><span class="sxs-lookup"><span data-stu-id="b5a30-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="b5a30-131">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="b5a30-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="b5a30-132">Transfert de la propriété d’un abonnement Azure</span><span class="sxs-lookup"><span data-stu-id="b5a30-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="b5a30-133">Déplacer des ressources vers un nouveau groupe de ressources ou un nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="b5a30-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="b5a30-134">Gérer les ressources à l’aide du portail Azure</span><span class="sxs-lookup"><span data-stu-id="b5a30-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
