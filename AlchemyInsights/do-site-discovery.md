---
title: Effectuer une détection du site
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529229"
---
# <a name="do-site-discovery"></a><span data-ttu-id="83cba-102">Effectuer une détection du site</span><span class="sxs-lookup"><span data-stu-id="83cba-102">Do site discovery</span></span>

<span data-ttu-id="83cba-103">Si votre organisation utilise toujours des applications web héritées et envisage utiliser le mode Internet Explorer (ce que la plupart des clients font), vous devez découvrir davantage de sites.</span><span class="sxs-lookup"><span data-stu-id="83cba-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="83cba-104">**Vous avez déjà déployé une version antérieure de Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="83cba-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="83cba-105">Si vous avez déjà configuré votre liste de sites d’entreprise pour qu’elle fonctionne avec la version héritée de Microsoft Edge, votre découverte de sites est alors quasiment terminé.</span><span class="sxs-lookup"><span data-stu-id="83cba-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="83cba-106">Il vous suffit d’ajouter des sites neutres.</span><span class="sxs-lookup"><span data-stu-id="83cba-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="83cba-107">Les sites neutres sont généralement des sites qui fournissent une authentification unique (SSO).</span><span class="sxs-lookup"><span data-stu-id="83cba-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="83cba-108">Si vous accédez à un site neutre à partir de Microsoft Edge, l’authentification se fera dans Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="83cba-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="83cba-109">Si vous accédez à un site neutre en mode Internet Explorer, l’authentification se fera en mode internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="83cba-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="83cba-110">Identifiez les sites SSO ou autres sites neutres que vous utilisez et ajoutez-les à votre liste de sites d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="83cba-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="83cba-111">**Internet Explorer est votre navigateur par défaut.**</span><span class="sxs-lookup"><span data-stu-id="83cba-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="83cba-112">Si vous avez commencé à utiliser Internet Explorer récemment, il est probable que vous ne sachiez pas les sites mis au niveau de sites web modernes mais qui exigent encore Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="83cba-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="83cba-113">Vous devez rechercher et ajouter ces sites à la liste des sites d’entreprise, afin d’utiliser Internet Explorer pour ces uniquement.</span><span class="sxs-lookup"><span data-stu-id="83cba-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="83cba-114">[Découverte de sites d’entreprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) découvre des sites qui pourraient nécessiter le mode Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="83cba-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="83cba-115">Il y a la possibilité de collecter des données sur les ordinateurs exécutant Windows Internet Explorer 8 à 11 sur Windows 10, Windows 8.1, ou Windows 7.</span><span class="sxs-lookup"><span data-stu-id="83cba-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="83cba-116">**Analyser les données**</span><span class="sxs-lookup"><span data-stu-id="83cba-116">**Analyze the data**</span></span>

<span data-ttu-id="83cba-117">Une fois que vous avez collecté les données de site, nous recommandons d’utiliser cette procédure à 4 étapes pour analyser les données :</span><span class="sxs-lookup"><span data-stu-id="83cba-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="83cba-118">Triez les données par domaine, puis par URL.</span><span class="sxs-lookup"><span data-stu-id="83cba-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="83cba-119">Définissez les limites d’une « application » à configurer en mode Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="83cba-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="83cba-120">Vous voulez inclure tous les sites et contrôles web qui définissent l’application, mais vous ne voulez pas inclure des sites et contrôles supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="83cba-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="83cba-121">Certains sites peuvent être aussi simples que *https://contoso.com/app1*, tandis que d’autres pourraient nécessiter la définition de plusieurs sites et pages.</span><span class="sxs-lookup"><span data-stu-id="83cba-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="83cba-122">Testez l’application pour vérifier qu’elle ne fonctionne pas en mode natif.</span><span class="sxs-lookup"><span data-stu-id="83cba-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="83cba-123">De nombreux sites proposent un contenu moderne lorsqu’ils détectent un navigateur moderne et du contenu hérité uniquement lorsqu’ils détectent Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="83cba-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="83cba-124">Ajoutez l’application à votre liste de sites d’entreprise en cas d’échec du test.</span><span class="sxs-lookup"><span data-stu-id="83cba-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="83cba-125">Il est recommandé de regrouper tous les sites qui composent une application.</span><span class="sxs-lookup"><span data-stu-id="83cba-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="83cba-126">Ainsi, lorsque vous mettez à niveau une application, il est plus facile de supprimer l’intégralité du site du mode Internet Explorer et de commencer à utiliser un navigateur moderne pour cette application.</span><span class="sxs-lookup"><span data-stu-id="83cba-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="83cba-127">Une fois que vous avez terminé la découverte de site et que vous avez analysé les données, vous pouvez  commencer à regarder la stratégie de canal.</span><span class="sxs-lookup"><span data-stu-id="83cba-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

