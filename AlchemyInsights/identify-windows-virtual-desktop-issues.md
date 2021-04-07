---
title: Identifier les problèmes liés à Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590276"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="6b6a2-102">Identifier les problèmes liés à Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="6b6a2-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="6b6a2-103">Windows Virtual Desktop Diagnostics n'utilise qu'une seule cmdlet PowerShell, mais contient de nombreux paramètres facultatifs qui permettent de circonscrire et d'isoler les problèmes.</span><span class="sxs-lookup"><span data-stu-id="6b6a2-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="6b6a2-104">Pour commencer :</span><span class="sxs-lookup"><span data-stu-id="6b6a2-104">To get started:</span></span> 

1. <span data-ttu-id="6b6a2-105">Téléchargez et importez le module PowerShell Windows Virtual Desktop.</span><span class="sxs-lookup"><span data-stu-id="6b6a2-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="6b6a2-106">Pour plus de détails, voir [Windows Virtual Desktop Cmdlets pour Windows PowerShell .](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="6b6a2-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="6b6a2-107">Exécutez le cmdlet suivant pour vous connecter à votre compte :</span><span class="sxs-lookup"><span data-stu-id="6b6a2-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="6b6a2-108">Exemple : `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="6b6a2-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="6b6a2-109">**REMARQUE :** Toutes les requêtes utilisant PowerShell doivent inclure les paramètres -UserName ou -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="6b6a2-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="6b6a2-110">Pour les capacités de surveillance, voir Utiliser [l'analyse des journaux pour la fonction de diagnostic](https://go.microsoft.com/fwlink/?linkid=2126847) .</span><span class="sxs-lookup"><span data-stu-id="6b6a2-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="6b6a2-111">Pour filtrer les activités de diagnostic par utilisateur, exécutez la cmdlet suivante :</span><span class="sxs-lookup"><span data-stu-id="6b6a2-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="6b6a2-112">Exemple : `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="6b6a2-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="6b6a2-113">Il existe une liste de filtres que vous pouvez exécuter pour diagnostiquer les problèmes.</span><span class="sxs-lookup"><span data-stu-id="6b6a2-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="6b6a2-114">Pour en savoir plus sur le diagnostic des problèmes, reportez-vous à la section [Identifier et diagnostiquer les problèmes de Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="6b6a2-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="6b6a2-115">Pour en savoir plus sur les erreurs courantes, consultez la rubrique [Scénarios d'erreurs courantes](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="6b6a2-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
