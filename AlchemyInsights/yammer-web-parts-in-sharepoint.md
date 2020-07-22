---
title: Composants WebPart Yammer dans SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157299"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="f0708-102">Composants WebPart Yammer dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="f0708-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="f0708-103">Les composants WebPart Conversations Yammer et Points forts Yammer améliorent la collaboration sur les pages SharePoint modernes et classiques.</span><span class="sxs-lookup"><span data-stu-id="f0708-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="f0708-104">Pour plus d’informations, voir [Conversations Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  et [points forts de Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span><span class="sxs-lookup"><span data-stu-id="f0708-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="f0708-105">Le composant WebPart Conversations Yammer moderne est mis à jour vers la nouvelle expérience Yammer et est disponible pour les clients ciblés pour la publication.</span><span class="sxs-lookup"><span data-stu-id="f0708-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="f0708-106">Le déploiement GA a commencé.</span><span class="sxs-lookup"><span data-stu-id="f0708-106">GA rollout has started.</span></span> <span data-ttu-id="f0708-107">Les nouvelles fonctionnalités incluent la possibilité de commencer une conversation avec n’importe quel billet (questions, sondages, compliments) et de marquer les réponses les plus directes directement à partir de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f0708-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="f0708-108">Pour plus d’informations, voir [Nouveau Yammer – Conditions d’utilisation et foire aux questions](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="f0708-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="f0708-109">Pour identifier les composants WebPart et la configuration qui vous sont appropriés, voir [Utiliser un composant WebPart Yammer dans SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="f0708-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="f0708-110">**Utilisation des composants WebPart avec SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="f0708-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="f0708-111">Les composants WebPart peuvent être utilisés dans des pages modernes et classiques au sein d’environnements locaux.</span><span class="sxs-lookup"><span data-stu-id="f0708-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="f0708-112">Pour plus d’informations sur les pages modernes, voir [Ajouter un flux Yammer à une page moderne dans SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="f0708-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="f0708-113">Pour plus d’informations sur les pages modernes, voir [Ajouter un flux Yammer à une page moderne dans SharePoint Server 2013, 2016 et 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="f0708-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="f0708-114">**Yammer Embed**</span><span class="sxs-lookup"><span data-stu-id="f0708-114">**Yammer Embed**</span></span>  

<span data-ttu-id="f0708-115">Utilisez l’outil de configuration Embed pour tester l’utilisation de Embed.</span><span class="sxs-lookup"><span data-stu-id="f0708-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="f0708-116">Une prochaine mise à jour de Embed permettra la nouvelle expérience Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0708-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="f0708-117">Pour plus d’informations, voir l’[outil de configuration de Yammer Embed](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="f0708-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="f0708-118">Pour mieux comprendre le composant de Yammer Embed, voir [Flux Embed](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="f0708-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="f0708-119">**Problèmes connus et limitations**</span><span class="sxs-lookup"><span data-stu-id="f0708-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="f0708-120">Les ID de groupe ne sont pas disponibles dans les nouvelles URL Yammer qui ont été modifiées.</span><span class="sxs-lookup"><span data-stu-id="f0708-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="f0708-121">Revenez en mode classique pour obtenir les ID de groupe ou d’autres ID d’URL.</span><span class="sxs-lookup"><span data-stu-id="f0708-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="f0708-122">Les domaines personnalisés (vanity) ne sont pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="f0708-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="f0708-123">Yammer Embed n’est pas optimisé pour les appareils mobiles.</span><span class="sxs-lookup"><span data-stu-id="f0708-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="f0708-124">Utilisez les pages modernes avec le composant WebPart Yammer Conversations pour une expérience optimale.</span><span class="sxs-lookup"><span data-stu-id="f0708-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="f0708-125">Les thèmes personnalisés peuvent affecter l’apparence et la facilité d’utilisation du composant WebPart Conversations sur Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0708-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="f0708-126">Ouvrez un cas de support pour signaler des problèmes.</span><span class="sxs-lookup"><span data-stu-id="f0708-126">Open a support case to report issues.</span></span>