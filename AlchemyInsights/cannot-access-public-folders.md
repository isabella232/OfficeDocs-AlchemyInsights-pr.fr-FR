---
title: Impossible d'accéder aux dossiers publics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819510"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="e0125-102">Outlook ne peut pas se connecter aux dossiers publics</span><span class="sxs-lookup"><span data-stu-id="e0125-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="e0125-103">Si l'accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="e0125-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="e0125-104">Connectez-vous à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d'utilisateur à problème pour qu'il corresponde au paramètre sur un compte d'utilisateur de travail.</span><span class="sxs-lookup"><span data-stu-id="e0125-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="e0125-105">Exemple :</span><span class="sxs-lookup"><span data-stu-id="e0125-105">Example:</span></span>

<span data-ttu-id="e0125-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="e0125-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="e0125-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="e0125-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="e0125-108">Attendez au moins une heure que la modification prenne effet.</span><span class="sxs-lookup"><span data-stu-id="e0125-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="e0125-109">Si le problème demeure, suivez cette procédure pour [résoudre](https://aka.ms/pfcte) les problèmes d'accès aux dossiers publics à l'aide d'Outlook.</span><span class="sxs-lookup"><span data-stu-id="e0125-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="e0125-110">**Pour contrôler les utilisateurs qui peuvent accéder aux dossiers publics à l'aide d'Outlook**:</span><span class="sxs-lookup"><span data-stu-id="e0125-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="e0125-111">Utiliser Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false</span><span class="sxs-lookup"><span data-stu-id="e0125-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="e0125-112">$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook</span><span class="sxs-lookup"><span data-stu-id="e0125-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="e0125-113">$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook.</span><span class="sxs-lookup"><span data-stu-id="e0125-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e0125-114">Ceci est la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="e0125-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="e0125-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="e0125-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="e0125-116">**Remarque** Cette procédure ne peut contrôler les connexions qu'avec les clients de bureau Outlook pour les clients Windows.</span><span class="sxs-lookup"><span data-stu-id="e0125-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e0125-117">Un utilisateur peut continuer à accéder aux dossiers publics à l'OWA ou Outlook pour Mac.</span><span class="sxs-lookup"><span data-stu-id="e0125-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="e0125-118">Pour plus d'informations, voir Annonce de la prise en [charge des connexions contrôlées aux dossiers publics dans Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="e0125-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>