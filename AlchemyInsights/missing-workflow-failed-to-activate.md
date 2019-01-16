---
title: Manque de flux de travail n’a pas pu activer
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288776"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="3c326-102">Manque de flux de travail n’a pas pu activer</span><span class="sxs-lookup"><span data-stu-id="3c326-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="3c326-103">Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (par exemple, « approbation - SharePoint 2010 ») à une liste ou une bibliothèque.</span><span class="sxs-lookup"><span data-stu-id="3c326-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3c326-104">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="3c326-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3c326-105">Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3c326-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3c326-106">**Objets du Site**, cliquez sur **flux de travail**.</span><span class="sxs-lookup"><span data-stu-id="3c326-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3c326-107">Dans la section **Nouveau** du ruban de **flux de travail** , sélectionnez le **Flux de travail réutilisable**.</span><span class="sxs-lookup"><span data-stu-id="3c326-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3c326-p101">Dans le formulaire de **Flux de travail réutilisable** , entrez le nom \*\* *Repair2010* \*\*. Pour **Type de plateforme**, cliquez sur **Flux de travail SharePoint 2010**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="3c326-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3c326-110">Dans la section **Enregistrer** du ruban de **flux de travail** , sélectionnez **Publier**.</span><span class="sxs-lookup"><span data-stu-id="3c326-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3c326-p102">Dans la section **Gérer** du ruban de **flux de travail** , sélectionnez **Publier globalement**. Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="3c326-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3c326-p103">Dans un navigateur web, recherchez le site Web racine de la collection de sites, puis accéder aux **Paramètres du Site** \> **Fonctionnalités de Collection de sites**. Ensuite, activer/désactiver la fonctionnalité de **flux de travail** :</span><span class="sxs-lookup"><span data-stu-id="3c326-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3c326-115">· Si la fonctionnalité est *activé* , cliquez sur **désactiver** et puis cliquez sur **Activer**.</span><span class="sxs-lookup"><span data-stu-id="3c326-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3c326-116">· Si la fonctionnalité est *désactivé* , cliquez sur **Activer**.</span><span class="sxs-lookup"><span data-stu-id="3c326-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3c326-117">Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.</span><span class="sxs-lookup"><span data-stu-id="3c326-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

