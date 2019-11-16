---
title: Dynamics 365-tableau de bord incorrect dans Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528549"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="045a6-102">Tableau de bord incorrect dans l’interface unifiée Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="045a6-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="045a6-103">Il existe plusieurs raisons pour lesquelles vous pouvez voir un tableau de bord différent de celui que vous attendez :</span><span class="sxs-lookup"><span data-stu-id="045a6-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="045a6-104">L’utilisateur a défini un tableau de bord par défaut de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="045a6-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="045a6-105">En règle générale, vous pouvez identifier un tableau de bord par défaut de l’utilisateur est défini si le bouton **définir par défaut** n’est pas affiché dans la barre de commandes tableau de bord.</span><span class="sxs-lookup"><span data-stu-id="045a6-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="045a6-106">Le tableau de bord par défaut de l’utilisateur remplacera tous les autres tableaux de bord par défaut, même si le tableau de bord par défaut de l’utilisateur ne se trouve pas dans l’application actuelle.</span><span class="sxs-lookup"><span data-stu-id="045a6-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="045a6-107">Utilisez la solution de contournement suivante pour annuler le tableau de bord par défaut.</span><span class="sxs-lookup"><span data-stu-id="045a6-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="045a6-108">Créez un tableau de bord personnel.</span><span class="sxs-lookup"><span data-stu-id="045a6-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="045a6-109">Définissez le nouveau tableau de bord comme utilisateur par défaut.</span><span class="sxs-lookup"><span data-stu-id="045a6-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="045a6-110">Supprimez ce tableau de bord.</span><span class="sxs-lookup"><span data-stu-id="045a6-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="045a6-111">Le tableau de bord est défini dans le sitemap.</span><span class="sxs-lookup"><span data-stu-id="045a6-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="045a6-112">Vous avez peut-être défini un tableau de bord par défaut de l’organisation en sélectionnant un tableau de bord et en choisissant « définir par défaut » sous « personnaliser le système ».</span><span class="sxs-lookup"><span data-stu-id="045a6-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="045a6-113">Toutefois, le tableau de bord défini dans le concepteur Sitemap est prioritaire sur ce tableau de bord, si l’utilisateur y a accès.</span><span class="sxs-lookup"><span data-stu-id="045a6-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="045a6-114">Pour que les utilisateurs voient le tableau de bord que vous avez défini en tant qu’organisation par défaut, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="045a6-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="045a6-115">Définir ce tableau de bord dans le plan de sitemap</span><span class="sxs-lookup"><span data-stu-id="045a6-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="045a6-116">Supprimer l’accès au tableau de bord défini sitemap pour ces utilisateurs</span><span class="sxs-lookup"><span data-stu-id="045a6-116">Remove access to the sitemap defined dashboard for those users</span></span>
