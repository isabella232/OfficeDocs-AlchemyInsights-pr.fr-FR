---
title: Échec de l’activation du flux de travail manquant
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667084"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="92e99-102">Échec de l’activation du flux de travail manquant</span><span class="sxs-lookup"><span data-stu-id="92e99-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="92e99-103">Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (tel que « approbation-SharePoint 2010 ») à une liste ou une bibliothèque.</span><span class="sxs-lookup"><span data-stu-id="92e99-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="92e99-104">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="92e99-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="92e99-105">Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="92e99-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="92e99-106">Sous **objets du site**, sélectionnez **flux de travail**.</span><span class="sxs-lookup"><span data-stu-id="92e99-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="92e99-107">Dans la section **nouveau** du ruban **flux de travail** , sélectionnez flux de travail **réutilisable**.</span><span class="sxs-lookup"><span data-stu-id="92e99-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="92e99-108">Dans le formulaire **créer un flux de travail réutilisable** , entrez le nom \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="92e99-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="92e99-109">Pour **type de plateforme**, cliquez sur **flux de travail SharePoint 2010**, puis sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="92e99-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="92e99-110">Dans la section **Enregistrer** du ruban **flux de travail** , sélectionnez **publier**.</span><span class="sxs-lookup"><span data-stu-id="92e99-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="92e99-111">Dans la section **gérer** du ruban **flux de travail** , sélectionnez **publier globalement**.</span><span class="sxs-lookup"><span data-stu-id="92e99-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="92e99-112">Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="92e99-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="92e99-113">Dans un navigateur Web, recherchez le site Web racine de la collection de sites, puis accédez aux **paramètres du site** fonctionnalités de la \> **collection de sites**.</span><span class="sxs-lookup"><span data-stu-id="92e99-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="92e99-114">Ensuite, activez ou désactivez la fonctionnalité **flux de travail** :</span><span class="sxs-lookup"><span data-stu-id="92e99-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="92e99-115">· Si la fonctionnalité est  *activée*  , cliquez sur désactiver **,** puis sur **activer**.</span><span class="sxs-lookup"><span data-stu-id="92e99-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="92e99-116">· Si la fonctionnalité est  *désactivée*  , cliquez sur **activer**.</span><span class="sxs-lookup"><span data-stu-id="92e99-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="92e99-117">Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.</span><span class="sxs-lookup"><span data-stu-id="92e99-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

