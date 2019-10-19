---
title: Problèmes de performances-SharePoint ou OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750554"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="9ff57-102">SharePoint ou OneDrive est lent, inaccessible ou indisponible pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9ff57-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="9ff57-103">Si un site OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui disposaient précédemment d’un accès, il peut y avoir un problème de service temporaire.</span><span class="sxs-lookup"><span data-stu-id="9ff57-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="9ff57-104">[Vérifiez le tableau de bord d’État du service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="9ff57-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="9ff57-105">**Ajouter et accorder une licence à l’utilisateur**</span><span class="sxs-lookup"><span data-stu-id="9ff57-105">**Add and license the user**</span></span>

<span data-ttu-id="9ff57-106">Vérifiez que vous [attribuez des licences aux utilisateurs dans Office 365 pour les entreprises](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="9ff57-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="9ff57-107">**Attribuer des autorisations**</span><span class="sxs-lookup"><span data-stu-id="9ff57-107">**Assign Permissions**</span></span>

<span data-ttu-id="9ff57-108">Si l’utilisateur a reçu une licence SharePoint et qu’il reçoit toujours un message de refus d’accès, vérifiez qu’il dispose du [niveau d’autorisation approprié](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="9ff57-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="9ff57-109">**Envisagez d’utiliser la fonctionnalité de demande d’accès**</span><span class="sxs-lookup"><span data-stu-id="9ff57-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="9ff57-110">La [fonctionnalité de demande d’accès](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permet aux utilisateurs de demander l’accès au contenu qu’ils n’ont pas actuellement le droit d’afficher.</span><span class="sxs-lookup"><span data-stu-id="9ff57-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="9ff57-111">**Autoriser le script personnalisé peut entraîner des problèmes de refus d’accès**</span><span class="sxs-lookup"><span data-stu-id="9ff57-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="9ff57-112">Il existe certains scénarios dans lesquels la fonctionnalité *autoriser les scripts personnalisés* peut présenter un accès refusé.</span><span class="sxs-lookup"><span data-stu-id="9ff57-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="9ff57-113">Pour obtenir la liste des fonctionnalités affectées, des considérations relatives à la sécurité et la possibilité de désactiver la fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="9ff57-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="9ff57-114">Visitez [ou bloquez le script personnalisé](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="9ff57-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

