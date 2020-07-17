---
title: Problèmes de licences Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146777"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="3bbb8-102">Problèmes de licences Yammer</span><span class="sxs-lookup"><span data-stu-id="3bbb8-102">Yammer licensing issues</span></span>

<span data-ttu-id="3bbb8-103">Tous les utilisateurs doivent disposer d’une licence pour pouvoir utiliser le service Yammer Enterprise. Toutefois, par défaut, Yammer n’exige pas que les utilisateurs disposent d’une licence pour accéder au service.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="3bbb8-104">Lorsqu’un administrateur modifie le paramètre pour bloquer les utilisateurs de Microsoft 365 sans licence Yammer, les utilisateurs qui ne disposent pas d’une licence Yammer Enterprise ne peuvent pas accéder au service Yammer.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="3bbb8-105">Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Gérer les licences utilisateur de Yammer dans Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="3bbb8-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="3bbb8-106">Lorsque les licences sont retirées aux utilisateurs, la vignette Yammer n’est plus affichée, et les autres services peuvent utiliser la suppression de la licence pour masquer les fonctionnalités.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="3bbb8-107">Dans d’autres cas, des fonctionnalités peuvent toujours apparaître, mais nécessitent une attribution de licence pour fonctionner.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="3bbb8-108">**La licence n’est pas mise à jour pour l’utilisateur**</span><span class="sxs-lookup"><span data-stu-id="3bbb8-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="3bbb8-109">Un utilisateur peut parfois se voir attribuer une licence sans toutefois réussir à accéder à Yammer.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="3bbb8-110">Les retards sont plus susceptibles de se produire lorsqu’une attribution de licence en masse est en cours.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="3bbb8-111">Les utilisateurs de Yammer peuvent ne pas être mis à jour dans le même ordre que les licences sont modifiées dans Azure AD car le système s’exécute de manière asynchrone.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="3bbb8-112">Patientez 24 heures avant d’ouvrir un cas de support technique pour signaler les problèmes de synchronisation des licences.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="3bbb8-113">**Attribution des licences en bloc**</span><span class="sxs-lookup"><span data-stu-id="3bbb8-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="3bbb8-114">Les licences peuvent être attribuées via le centre d’administration ou l’écriture de scripts PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="3bbb8-115">Si vous souhaitez en savoir plus, veuillez consulter les rubriques [Attribuer des licences aux utilisateurs](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) et [Attribuer des licences à des comptes d’utilisateurs avec Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="3bbb8-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="3bbb8-116">Le support Microsoft ne fournit aucune aide sur la création de scripts, mais la documentation sur l’attribution des licences Yammer est disponible.</span><span class="sxs-lookup"><span data-stu-id="3bbb8-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="3bbb8-117">Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Gérer les licences Yammer à l’aide de Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="3bbb8-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>