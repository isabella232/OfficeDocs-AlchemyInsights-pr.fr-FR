---
title: Le flux de travail ne démarre pas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403741"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="e212a-102">Le flux de travail ne démarre pas</span><span class="sxs-lookup"><span data-stu-id="e212a-102">Workflow is not starting</span></span>

- <span data-ttu-id="e212a-103">Les flux de travail SharePoint 2010 et SharePoint 2013 ne démarrent pas.</span><span class="sxs-lookup"><span data-stu-id="e212a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="e212a-104">Si votre flux de travail ne démarre pas, il peut y avoir un problème de service temporaire dans lequel les utilisateurs peuvent faire face à des retards intermittents avec la progression du flux de travail.</span><span class="sxs-lookup"><span data-stu-id="e212a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="e212a-105">Consultez le [tableau de bord d’état](https://admin.microsoft.com/AdminPortal/Home/servicehealth) du service pour voir si votre organisation est impactée.</span><span class="sxs-lookup"><span data-stu-id="e212a-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="e212a-106">Si plus de 24 heures se sont écoulées depuis le premier problème, veuillez enregistrer un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="e212a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e212a-107">Dans de nombreux cas, nous travaillons déjà sur une solution.</span><span class="sxs-lookup"><span data-stu-id="e212a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e212a-108">Veuillez nous donner au moins 24 heures pour terminer une solution.</span><span class="sxs-lookup"><span data-stu-id="e212a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="e212a-109">Les flux de travail SharePoint 2010 ont été retardés au démarrage.</span><span class="sxs-lookup"><span data-stu-id="e212a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="e212a-110">Cela se produit si le flux de travail est déclenché par lots importants.</span><span class="sxs-lookup"><span data-stu-id="e212a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="e212a-111">(par exemple, lorsque plusieurs éléments sont ajoutés en même temps).</span><span class="sxs-lookup"><span data-stu-id="e212a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="e212a-112">Les flux de travail ne sont pas conçus pour s’exécuter en temps réel. Un délai est donc un comportement par conception.</span><span class="sxs-lookup"><span data-stu-id="e212a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="e212a-113">Si le flux de travail est un langage X WORKFLOW (Extensible Object Markup Language) complexe, la compilation peut être lente.</span><span class="sxs-lookup"><span data-stu-id="e212a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="e212a-114">Consultez [cet](https://support.microsoft.com//kb/3043697) article.</span><span class="sxs-lookup"><span data-stu-id="e212a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="e212a-115">Vous devez simplifier le flux de travail ou le reconçre à l’aide du type de plateforme de flux de travail Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="e212a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="e212a-116">Si l’historique de votre flux de travail est devenu important, vous pouvez vider les éléments ou créer une liste d’historique.</span><span class="sxs-lookup"><span data-stu-id="e212a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="e212a-117">Plus d’informations : [Vider l’historique des flux de travail](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="e212a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="e212a-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e212a-118">Related topics</span></span>
<span data-ttu-id="e212a-119">Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?</span><span class="sxs-lookup"><span data-stu-id="e212a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e212a-120">Créer un flux</span><span class="sxs-lookup"><span data-stu-id="e212a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e212a-121">SharePoint et Flow</span><span class="sxs-lookup"><span data-stu-id="e212a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
