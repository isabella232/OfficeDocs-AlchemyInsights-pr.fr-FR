---
title: 2609-Retention-or-eDiscovery-Holding
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994062"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="5198a-102">Impossible de supprimer des éléments dans SharePoint Online ou OneDrive entreprise</span><span class="sxs-lookup"><span data-stu-id="5198a-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="5198a-103">Vous ou vos utilisateurs pouvez ne pas être en mesure de supprimer des éléments dans SharePoint Online ou OneDrive entreprise, car une stratégie de rétention, une étiquette de rétention ou une conservation eDiscovery est appliquée à un site SharePoint ou à un élément spécifique.</span><span class="sxs-lookup"><span data-stu-id="5198a-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="5198a-104">Il s’agit notamment de l’impossibilité de supprimer un document, une version d’un document, un dossier, une bibliothèque de documents, une liste, une application, un site ou une collection de sites.</span><span class="sxs-lookup"><span data-stu-id="5198a-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="5198a-105">Voici quelques exemples de messages d’erreur que vous pouvez recevoir si vous essayez de supprimer un élément qui est conservé :</span><span class="sxs-lookup"><span data-stu-id="5198a-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="5198a-106">« Ce site ne peut pas être supprimé, car il est inclus dans une conservation eDiscovery ou une stratégie de rétention »</span><span class="sxs-lookup"><span data-stu-id="5198a-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="5198a-107">« Ce site a une stratégie de conformité définie sur bloquer la suppression »</span><span class="sxs-lookup"><span data-stu-id="5198a-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="5198a-108">« Une stratégie de conformité bloque actuellement cette suppression de site »</span><span class="sxs-lookup"><span data-stu-id="5198a-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="5198a-109">« Cette collection de sites ne peut pas être supprimée car elle contient des sites inclus dans une conservation eDiscovery ou une stratégie de rétention »</span><span class="sxs-lookup"><span data-stu-id="5198a-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="5198a-110">« Vous devez supprimer tous les éléments de ce dossier avant de supprimer le dossier »</span><span class="sxs-lookup"><span data-stu-id="5198a-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="5198a-111">« Les versions de cet élément ne peuvent pas être supprimées, car il s’agit d’une stratégie de rétention ou de conservation »</span><span class="sxs-lookup"><span data-stu-id="5198a-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="5198a-112">« L’élément ne peut pas être supprimé en conservation »</span><span class="sxs-lookup"><span data-stu-id="5198a-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="5198a-113">"L’étiquette appliquée à cet élément l’empêche d’être modifiée ou supprimée."</span><span class="sxs-lookup"><span data-stu-id="5198a-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="5198a-114">« La liste ne peut pas être supprimée lors de la conservation ou de la stratégie de rétention »</span><span class="sxs-lookup"><span data-stu-id="5198a-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="5198a-115">« La liste ne peut pas être supprimée si elle est bloquée ou si une stratégie de rétention lui est appliquée »</span><span class="sxs-lookup"><span data-stu-id="5198a-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="5198a-116">Pour supprimer des éléments dans l’un de ces scénarios, la stratégie de rétention, l’étiquette de rétention ou le blocage eDiscovery doit être supprimé (ou un site doit être exclu d’une stratégie de rétention).</span><span class="sxs-lookup"><span data-stu-id="5198a-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="5198a-117">Vous devez désactiver ou exclure le blocage respectif qui est à l’origine de ce problème.</span><span class="sxs-lookup"><span data-stu-id="5198a-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="5198a-118">Après la suppression d’une stratégie de rétention ou d’une conservation, la modification peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="5198a-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="5198a-119">Pour plus d’informations sur les différentes fonctionnalités de rétention et de conservation pouvant être appliquées aux sites SharePoint et aux comptes OneDrive, consultez l’une des rubriques suivantes.</span><span class="sxs-lookup"><span data-stu-id="5198a-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="5198a-120">Vue d’ensemble des stratégies de rétention</span><span class="sxs-lookup"><span data-stu-id="5198a-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="5198a-121">Vue d’ensemble des étiquettes de rétention</span><span class="sxs-lookup"><span data-stu-id="5198a-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="5198a-122">Gérer les suspensions dans Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="5198a-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="5198a-123">conservations eDiscovery</span><span class="sxs-lookup"><span data-stu-id="5198a-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="5198a-124">Stratégies de fermeture et de suppression de site héritées</span><span class="sxs-lookup"><span data-stu-id="5198a-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
