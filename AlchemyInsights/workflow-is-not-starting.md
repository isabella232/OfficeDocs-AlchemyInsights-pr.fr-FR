---
title: Le flux de travail ne démarre pas
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738087"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="5159e-102">Le flux de travail ne démarre pas</span><span class="sxs-lookup"><span data-stu-id="5159e-102">Workflow is not starting</span></span>

- <span data-ttu-id="5159e-103">Les flux de travail SharePoint 2010 et SharePoint 2013 ne démarrent pas.</span><span class="sxs-lookup"><span data-stu-id="5159e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="5159e-104">Si votre flux de travail ne démarre pas, il peut y avoir un problème de service temporaire dans lequel les utilisateurs peuvent observer des retards intermittents avec la progression du flux de travail.</span><span class="sxs-lookup"><span data-stu-id="5159e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="5159e-105">Consultez le [tableau de bord d’État du service](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pour voir si votre organisation est concernée.</span><span class="sxs-lookup"><span data-stu-id="5159e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="5159e-106">Si plus de 24 heures se sont écoulées depuis le début de ce problème, veuillez consigner un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="5159e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="5159e-107">Dans de nombreux cas, nous travaillons déjà sur une solution.</span><span class="sxs-lookup"><span data-stu-id="5159e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="5159e-108">Veuillez nous fournir au moins 24 heures pour terminer une solution.</span><span class="sxs-lookup"><span data-stu-id="5159e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="5159e-109">Flux de travail SharePoint 2010 retardés au démarrage.</span><span class="sxs-lookup"><span data-stu-id="5159e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="5159e-110">Cela se produit si le flux de travail est déclenché par des lots volumineux.</span><span class="sxs-lookup"><span data-stu-id="5159e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="5159e-111">(par exemple, lorsque plusieurs éléments sont ajoutés à la fois).</span><span class="sxs-lookup"><span data-stu-id="5159e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="5159e-112">Les flux de travail ne sont pas conçus pour s’exécuter en temps réel, c’est pourquoi un délai est le comportement par défaut.</span><span class="sxs-lookup"><span data-stu-id="5159e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="5159e-113">Si le flux de travail est complexe Extensible Object Markup Language (XMOL), la compilation peut être lente.</span><span class="sxs-lookup"><span data-stu-id="5159e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="5159e-114">Consultez [cet](https://support.microsoft.com//kb/3043697) article.</span><span class="sxs-lookup"><span data-stu-id="5159e-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="5159e-115">Vous devez simplifier le flux de travail ou le reconcevoir à l’aide du type de plateforme de flux de travail Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="5159e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="5159e-116">Si l’historique de votre flux de travail s’est agrandi, vous souhaiterez peut-être purger les éléments ou créer un historique.</span><span class="sxs-lookup"><span data-stu-id="5159e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="5159e-117">Pour plus d’informations : [purger l’historique du flux de travail](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="5159e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="5159e-118">Sujets associés</span><span class="sxs-lookup"><span data-stu-id="5159e-118">Related topics</span></span>
<span data-ttu-id="5159e-119">Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?</span><span class="sxs-lookup"><span data-stu-id="5159e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5159e-120">Créer un flux</span><span class="sxs-lookup"><span data-stu-id="5159e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5159e-121">SharePoint et flux</span><span class="sxs-lookup"><span data-stu-id="5159e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


