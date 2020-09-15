---
title: Migration des étiquettes AIP vers un étiquetage unifié/MIP dans le Centre de conformité
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674324"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="b990d-102">Migration des étiquettes AIP vers un étiquetage unifié/MIP dans le Centre de conformité</span><span class="sxs-lookup"><span data-stu-id="b990d-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="b990d-103">Pour migrer des étiquettes AIP vers un étiquetage unifié dans le Centre de sécurité et de conformité, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="b990d-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="b990d-104">**Activer la protection à partir du portail Azure**</span><span class="sxs-lookup"><span data-stu-id="b990d-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="b990d-105">Si vous ne l’avez pas encore fait, ouvrez une nouvelle fenêtre de navigateur et [Connectez-vous au portail Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="b990d-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="b990d-106">Accédez au panneau **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="b990d-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="b990d-107">Par exemple, dans le menu hub, cliquez sur **Tous les services** et commencez à taper **Informations** dans la zone de filtre.</span><span class="sxs-lookup"><span data-stu-id="b990d-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="b990d-108">Sélectionnez **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="b990d-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="b990d-109">Si vous n’avez pas jamais accédé au panneau Azure Information Protection, consultez les [étapes supplémentaires](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pour l’ajouter au portail.</span><span class="sxs-lookup"><span data-stu-id="b990d-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="b990d-110">Pour ouvrir le panneau d’Azure Information Protection, vous devez disposer d’un plan [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou d’une offre Office 365 incluant Rights Management.</span><span class="sxs-lookup"><span data-stu-id="b990d-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="b990d-111">Si vous avez l’un de ces abonnements, mais que vous voyez un message indiquant qu’un abonnement valide est introuvable, [Contacter l’Aide et support Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ou utiliser vos canaux de support standard.</span><span class="sxs-lookup"><span data-stu-id="b990d-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="b990d-112">Recherchez les options du menu **Gérer**, puis sélectionnez **activation de la protection**.</span><span class="sxs-lookup"><span data-stu-id="b990d-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="b990d-113">Cliquez sur **Activer**, puis confirmez votre action.</span><span class="sxs-lookup"><span data-stu-id="b990d-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="b990d-114">Une fois l’activation terminée, la barre d’informations affiche **L’activation s’est correctement terminée**.</span><span class="sxs-lookup"><span data-stu-id="b990d-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="b990d-115">**Migrer des étiquettes Azure Information Protection vers le Centre de sécurité et conformité Office 365**</span><span class="sxs-lookup"><span data-stu-id="b990d-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="b990d-116">Vérifiez que vous êtes connecté en tant qu’utilisateur disposant des autorisations d’administrateur général.</span><span class="sxs-lookup"><span data-stu-id="b990d-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="b990d-117">Accédez au panneau **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="b990d-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="b990d-118">À partir de l’option de menu **Gérer**, sélectionnez **Étiquetage unifié**.</span><span class="sxs-lookup"><span data-stu-id="b990d-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="b990d-119">Sur le panneau **Azure Information Protection – Étiquetage unifié**, cliquez sur **Activer** et suivez les instructions en ligne.</span><span class="sxs-lookup"><span data-stu-id="b990d-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="b990d-120">**Remarque**: Vérifiez que vous disposez des autorisations appropriées avant d’activer la migration du Centre de sécurité et conformité.</span><span class="sxs-lookup"><span data-stu-id="b990d-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="b990d-121">Pour plus d’informations, voir les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="b990d-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="b990d-122">Est-ce que je dois être un administrateur général pour configurer Azure Information Protection, ou puis-je déléguer aux autres administrateurs ?</span><span class="sxs-lookup"><span data-stu-id="b990d-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="b990d-123">Informations importantes sur les rôles d’administrateur après la migration vers le Centre de sécurité et conformité.</span><span class="sxs-lookup"><span data-stu-id="b990d-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="b990d-124">Pour plus d’informations sur la migration des AIP vers l’étiquetage unifié dans le Centre de sécurité et conformité, voir [Migrer des étiquettes](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="b990d-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
