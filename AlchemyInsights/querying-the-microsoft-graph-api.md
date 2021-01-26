---
title: Interrogation de l’API Microsoft Graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950713"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="2a282-102">Interrogation de l’API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="2a282-103">Cette rubrique peut également s’appliquer aux développeurs qui utilisent encore l’API Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="2a282-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="2a282-104">Toutefois, il **est vivement recommandé** d’utiliser Microsoft Graph pour tous vos scénarios de gestion des répertoires, des identités et des accès.</span><span class="sxs-lookup"><span data-stu-id="2a282-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="2a282-105">**Problèmes d’authentification ou d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="2a282-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="2a282-106">Si votre  application ne parvient pas à acquérir des jetons pour appeler Microsoft Graph, sélectionnez Problème d’obtention d’une catégorie de jeton d’accès **(authentification)** Microsoft Graph pour obtenir une aide et un support plus spécifiques sur cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="2a282-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="2a282-107">Si votre application reçoit des erreurs d’autorisation **401 ou 403** lors de l’appel de Microsoft Graph, sélectionnez la catégorie d’API Microsoft Graph Obtention d’une erreur d’accès refusé **(autorisation)** pour obtenir une aide et un support plus spécifiques sur cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="2a282-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="2a282-108">**Je veux utiliser Microsoft Graph, mais je ne sais pas par où commencer**</span><span class="sxs-lookup"><span data-stu-id="2a282-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="2a282-109">Pour en savoir plus sur Microsoft Graph, voir :</span><span class="sxs-lookup"><span data-stu-id="2a282-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="2a282-110">Présentation de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="2a282-111">Vue d’ensemble de la gestion des identités et des accès dans Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="2a282-112">Commencer à créer des applications Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="2a282-113">**Explorateur Microsoft Graph** : tester les API Microsoft Graph dans votre client ou un client de démonstration</span><span class="sxs-lookup"><span data-stu-id="2a282-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="2a282-114">**Je veux utiliser Microsoft Graph, mais prend-il en charge les API d’annuaire v1.0 dont j’ai besoin ?**</span><span class="sxs-lookup"><span data-stu-id="2a282-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="2a282-115">Microsoft Graph est l’API recommandée pour la gestion des répertoires, des identités et des accès.</span><span class="sxs-lookup"><span data-stu-id="2a282-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="2a282-116">Toutefois, il existe encore quelques lacunes entre ce qui est possible dans Azure AD Graph et Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2a282-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="2a282-117">Lisez les articles suivants, qui mettent en évidence les différences les plus à jour pour vous aider dans votre choix :</span><span class="sxs-lookup"><span data-stu-id="2a282-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="2a282-118">Différences de type de ressource entre Azure AD Graph et Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="2a282-119">Différences de propriétés entre Azure AD Graph et Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="2a282-120">Différences de méthode entre Azure AD et Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="2a282-121">**Lorsque j’interroge *l’objet utilisateur,* la plupart de ses propriétés sont manquantes**</span><span class="sxs-lookup"><span data-stu-id="2a282-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="2a282-122">`GET https://graph.microsoft.com/v1.0/users` renvoie uniquement 11 propriétés, car Microsoft Graph sélectionne automatiquement un ensemble par défaut *de* propriétés utilisateur à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="2a282-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="2a282-123">Si vous avez besoin *d’autres* propriétés utilisateur, utilisez $select pour sélectionner les propriétés dont votre application a besoin.</span><span class="sxs-lookup"><span data-stu-id="2a282-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="2a282-124">Essayez d’abord **dans l’Explorateur Microsoft Graph.**</span><span class="sxs-lookup"><span data-stu-id="2a282-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="2a282-125">**Certaines valeurs de propriété utilisateur *sont null* même si je sais qu’elles sont définies**</span><span class="sxs-lookup"><span data-stu-id="2a282-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="2a282-126">L’explication la plus probable est que l’application a reçu l’autorisation *User.ReadBasic.All.*</span><span class="sxs-lookup"><span data-stu-id="2a282-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="2a282-127">Cela permet à l’application de lire un ensemble limité de propriétés utilisateur, renvoyant toutes les autres propriétés comme null, même si elles ont été définies précédemment.</span><span class="sxs-lookup"><span data-stu-id="2a282-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="2a282-128">Essayez plutôt d’accorder *l’autorisation User.Read.All* à l’application.</span><span class="sxs-lookup"><span data-stu-id="2a282-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="2a282-129">Pour plus d’informations, [consultez les autorisations utilisateur de Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="2a282-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="2a282-130">**J’ai des difficultés à utiliser les paramètres de requête OData pour filtrer des données dans mes demandes**</span><span class="sxs-lookup"><span data-stu-id="2a282-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="2a282-131">Bien que Microsoft Graph prend en charge un large éventail de paramètres de requête OData, la plupart de ces paramètres ne sont pas entièrement pris en charge par les services d’annuaire (ressources qui héritent de *directoryObject*) dans Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2a282-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="2a282-132">Les mêmes limitations qui étaient présentes dans Azure AD Graph persistent pour la plupart dans Microsoft Graph :</span><span class="sxs-lookup"><span data-stu-id="2a282-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="2a282-133">**Non pris en** charge : $count, $search et $filter sur des valeurs *null* *ou non null*</span><span class="sxs-lookup"><span data-stu-id="2a282-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="2a282-134">**Non pris en** charge : $filter sur certaines propriétés (voir les rubriques de ressources sur lesquelles les propriétés sont filtrables)</span><span class="sxs-lookup"><span data-stu-id="2a282-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="2a282-135">**Non pris en** charge : pagination, filtrage et tri en même temps</span><span class="sxs-lookup"><span data-stu-id="2a282-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="2a282-136">**Non pris en** charge : filtrage sur une relation.</span><span class="sxs-lookup"><span data-stu-id="2a282-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="2a282-137">Par exemple, recherchez tous les membres du groupe d’ingénierie qui se trouvent au Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="2a282-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="2a282-138">**Prise en charge** partielle : $orderby sur *l’utilisateur* (displayName et userPrincipalName uniquement) et le *groupe*</span><span class="sxs-lookup"><span data-stu-id="2a282-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="2a282-139">Prise en charge partielle : $filter (prend en charge uniquement *eq* *,* *startswith*, or , and , *and* limited *any*) support, $expand (le développement des relations d’un seul objet renvoie toutes les relations, mais le développement d’une collection de relations d’objets est limité)</span><span class="sxs-lookup"><span data-stu-id="2a282-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="2a282-140">Pour plus d’informations, voir [Personnaliser les réponses avec les paramètres de requête.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="2a282-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="2a282-141">**L’API que j’appelle ne fonctionne pas: où puis-je faire d’autres tests ?**</span><span class="sxs-lookup"><span data-stu-id="2a282-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="2a282-142">**Explorateur Microsoft Graph** : testez les API Microsoft Graph dans  votre client ou un client de démonstration et consultez également les exemples de requêtes dans l’Explorateur Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2a282-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="2a282-143">**Lorsque j’interroge des données, j’ai l’impression d’obtenir un jeu de données incomplet**</span><span class="sxs-lookup"><span data-stu-id="2a282-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="2a282-144">Si vous interrogez une collection (comme les utilisateurs), Microsoft Graph utilise des limites de page côté serveur afin que les résultats soient toujours renvoyés avec une taille de page par défaut.</span><span class="sxs-lookup"><span data-stu-id="2a282-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="2a282-145">Votre application doit toujours s’attendre à passer en page les collections renvoyées par le service.</span><span class="sxs-lookup"><span data-stu-id="2a282-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="2a282-146">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="2a282-146">For more information, see:</span></span>

- [<span data-ttu-id="2a282-147">Meilleures pratiques de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="2a282-148">Pagination des données Microsoft Graph dans votre application</span><span class="sxs-lookup"><span data-stu-id="2a282-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="2a282-149">**Mon application est trop lente et est également limitée. Quelles améliorations puis-je apporter ?**</span><span class="sxs-lookup"><span data-stu-id="2a282-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="2a282-150">Selon votre scénario, différentes options sont à votre disposition pour rendre votre application plus performante et, dans certains cas, moins susceptible d’être limitée par le service (lorsque vous faites trop d’appels).</span><span class="sxs-lookup"><span data-stu-id="2a282-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="2a282-151">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="2a282-151">To learn more, see:</span></span>

- [<span data-ttu-id="2a282-152">Meilleures pratiques de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="2a282-153">Demandes de traitement par lots</span><span class="sxs-lookup"><span data-stu-id="2a282-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="2a282-154">Suivre les modifications par le biais d’une requête delta</span><span class="sxs-lookup"><span data-stu-id="2a282-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="2a282-155">Être averti des modifications par le biais de webhooks</span><span class="sxs-lookup"><span data-stu-id="2a282-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="2a282-156">Recommandations en cas de limitation</span><span class="sxs-lookup"><span data-stu-id="2a282-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="2a282-157">**Où puis-je trouver plus d’informations sur les erreurs et les problèmes connus ?**</span><span class="sxs-lookup"><span data-stu-id="2a282-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="2a282-158">Informations sur la réponse d’erreur Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="2a282-159">Problèmes connus avec Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a282-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="2a282-160">**Où puis-je vérifier l’état de la disponibilité et de la connectivité du service ?**</span><span class="sxs-lookup"><span data-stu-id="2a282-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="2a282-161">La disponibilité et la connectivité des services sous-jacents accessibles via Microsoft Graph peuvent avoir un impact sur la disponibilité et les performances globales de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2a282-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="2a282-162">Pour l’état du service Azure Active Directory, vérifiez l’état des services **Sécurité + Identité** répertoriés dans la page [d’état Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="2a282-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="2a282-163">Pour les services Office qui contribuent à Microsoft Graph, vérifiez l’état des services répertoriés dans le tableau de bord d’état du [service Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="2a282-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
