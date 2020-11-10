---
title: Commentaires sur les éléments de liste
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947487"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="28437-102">Commentaires sur les éléments de liste</span><span class="sxs-lookup"><span data-stu-id="28437-102">Comments on List items</span></span>

<span data-ttu-id="28437-103">Les utilisateurs seront rapidement en mesure d’ajouter et de supprimer des commentaires sur les éléments de liste.</span><span class="sxs-lookup"><span data-stu-id="28437-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="28437-104">Les utilisateurs peuvent afficher tous les commentaires sur un élément de liste et filtrer entre les affichages affichant des commentaires ou des activités liées à un élément.</span><span class="sxs-lookup"><span data-stu-id="28437-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="28437-105">**Minutage** :</span><span class="sxs-lookup"><span data-stu-id="28437-105">**Timing** :</span></span>

<span data-ttu-id="28437-106">**Publication ciblée** : déploiement progressif à mi-octobre et attendu à mi-novembre</span><span class="sxs-lookup"><span data-stu-id="28437-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="28437-107">**Version standard** : déploiement graduel en milieu de novembre et attendu au début du 1er décembre</span><span class="sxs-lookup"><span data-stu-id="28437-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="28437-108">**Déploiement** : version ciblée pour l’ensemble de l’Organisation</span><span class="sxs-lookup"><span data-stu-id="28437-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="28437-109">Les utilisateurs doivent noter les points suivants avant de pouvoir ajouter et supprimer des commentaires :</span><span class="sxs-lookup"><span data-stu-id="28437-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="28437-110">Les commentaires suivent les paramètres d’autorisation inhérents à SharePoint.</span><span class="sxs-lookup"><span data-stu-id="28437-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="28437-111">Les listes classiques qui ne sont pas encore conçues pour être affichées dans les interfaces utilisateur modernes, comme les listes de tâches, ne disposent pas de cette fonctionnalité de commentaire.</span><span class="sxs-lookup"><span data-stu-id="28437-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="28437-112">La mise en commentaire sur des listes dans teams n’est pas disponible dans cette version.</span><span class="sxs-lookup"><span data-stu-id="28437-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="28437-113">Les commentaires ne sont pas indexés par la recherche.</span><span class="sxs-lookup"><span data-stu-id="28437-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="28437-114">Les administrateurs peuvent désactiver cette fonctionnalité au niveau de l’organisation en modifiant le paramètre **CommentsOnListItemsDisabled** dans l’applet de commande **Set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28437-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="28437-115">Il n’est pas possible actuellement de désactiver les commentaires au niveau du site ou de la liste.</span><span class="sxs-lookup"><span data-stu-id="28437-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="28437-116">Nous espérons que ces contrôles doivent être mis à jour plus tard au cours du premier trimestre 2021.</span><span class="sxs-lookup"><span data-stu-id="28437-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
