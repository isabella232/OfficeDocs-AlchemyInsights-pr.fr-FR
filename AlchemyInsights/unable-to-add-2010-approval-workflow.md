---
title: Impossible d’ajouter le flux de travail d’approbation 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748682"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="9b2f9-102">Impossible d’ajouter le flux de travail d’approbation 2010</span><span class="sxs-lookup"><span data-stu-id="9b2f9-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="9b2f9-103">Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (tel que « approbation-SharePoint 2010 ») à une liste ou une bibliothèque.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9b2f9-104">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="9b2f9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9b2f9-105">Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9b2f9-106">Sous **objets du site**, sélectionnez **flux de travail**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9b2f9-107">Dans la section **nouveau** du ruban **flux de travail** , sélectionnez flux de travail **réutilisable**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9b2f9-108">Dans le formulaire **créer un flux de travail réutilisable** , entrez le nom \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="9b2f9-109">Pour **type de plateforme**, cliquez sur **flux de travail SharePoint 2010**, puis sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9b2f9-110">Dans la section **Enregistrer** du ruban **flux de travail** , sélectionnez **publier**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9b2f9-111">Dans la section **gérer** du ruban **flux de travail** , sélectionnez **publier globalement**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="9b2f9-112">Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9b2f9-113">Dans un navigateur Web, recherchez le site Web racine de la collection de sites, puis accédez aux **paramètres** \> du site fonctionnalités de la **collection de sites**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="9b2f9-114">Activer/désactiver la fonctionnalité **flux de travail** :</span><span class="sxs-lookup"><span data-stu-id="9b2f9-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9b2f9-115">· Si la fonctionnalité est *activée* , cliquez sur désactiver **,** puis sur **activer**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9b2f9-116">· Si la fonctionnalité est *désactivée* , cliquez sur **activer**.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9b2f9-117">Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.</span><span class="sxs-lookup"><span data-stu-id="9b2f9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

