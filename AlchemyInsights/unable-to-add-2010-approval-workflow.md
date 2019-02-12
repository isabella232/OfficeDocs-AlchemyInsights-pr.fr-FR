---
title: Impossible d’ajouter le flux de travail approbation 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925414"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="35efa-102">Impossible d’ajouter le flux de travail approbation 2010</span><span class="sxs-lookup"><span data-stu-id="35efa-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="35efa-103">Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (par exemple, « approbation - SharePoint 2010 ») à une liste ou une bibliothèque.</span><span class="sxs-lookup"><span data-stu-id="35efa-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="35efa-104">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="35efa-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="35efa-105">Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="35efa-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="35efa-106">**Objets du Site**, cliquez sur **flux de travail**.</span><span class="sxs-lookup"><span data-stu-id="35efa-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="35efa-107">Dans la section **Nouveau** du ruban de **flux de travail** , sélectionnez le **Flux de travail réutilisable**.</span><span class="sxs-lookup"><span data-stu-id="35efa-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="35efa-p101">Dans le formulaire de **Flux de travail réutilisable** , entrez le nom \*\* *Repair2010* \*\*. Pour **Type de plateforme**, cliquez sur **Flux de travail SharePoint 2010**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="35efa-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="35efa-110">Dans la section **Enregistrer** du ruban de **flux de travail** , sélectionnez **Publier**.</span><span class="sxs-lookup"><span data-stu-id="35efa-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="35efa-p102">Dans la section **Gérer** du ruban de **flux de travail** , sélectionnez **Publier globalement**. Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="35efa-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="35efa-p103">Dans un navigateur web, recherchez le site Web racine de la collection de sites, puis accéder aux **Paramètres du Site** \> **Fonctionnalités de Collection de sites**. Activer/désactiver la fonctionnalité de **flux de travail** :</span><span class="sxs-lookup"><span data-stu-id="35efa-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="35efa-115">· Si la fonctionnalité est *activé* , cliquez sur **désactiver** et puis cliquez sur **Activer**.</span><span class="sxs-lookup"><span data-stu-id="35efa-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="35efa-116">· Si la fonctionnalité est *désactivé* , cliquez sur **Activer**.</span><span class="sxs-lookup"><span data-stu-id="35efa-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="35efa-117">Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.</span><span class="sxs-lookup"><span data-stu-id="35efa-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

