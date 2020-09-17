---
title: Impossible d’accéder aux dossiers publics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812545"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="06c7e-102">Outlook ne peut pas se connecter aux dossiers publics</span><span class="sxs-lookup"><span data-stu-id="06c7e-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="06c7e-103">Si l’accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="06c7e-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="06c7e-104">Connectez-vous à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d’utilisateur posant problème pour qu’il corresponde au paramètre sur un compte d’utilisateur de travail.</span><span class="sxs-lookup"><span data-stu-id="06c7e-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="06c7e-105">Exemple :</span><span class="sxs-lookup"><span data-stu-id="06c7e-105">Example:</span></span>

<span data-ttu-id="06c7e-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="06c7e-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="06c7e-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="06c7e-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="06c7e-108">Patientez au moins une heure pour que la modification prenne effet.</span><span class="sxs-lookup"><span data-stu-id="06c7e-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="06c7e-109">Si le problème persiste, suivez [cette procédure](https://aka.ms/pfcte) pour résoudre les problèmes d’accès aux dossiers publics à l’aide d’Outlook.</span><span class="sxs-lookup"><span data-stu-id="06c7e-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="06c7e-110">**Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook**:</span><span class="sxs-lookup"><span data-stu-id="06c7e-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="06c7e-111">Utilisation de Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false</span><span class="sxs-lookup"><span data-stu-id="06c7e-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="06c7e-112">$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook</span><span class="sxs-lookup"><span data-stu-id="06c7e-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="06c7e-113">$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook.</span><span class="sxs-lookup"><span data-stu-id="06c7e-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="06c7e-114">Ceci est la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="06c7e-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="06c7e-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="06c7e-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="06c7e-116">**Note** Cette procédure permet de contrôler les connexions uniquement avec les clients Outlook pour ordinateur de bureau pour Windows.</span><span class="sxs-lookup"><span data-stu-id="06c7e-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="06c7e-117">Un utilisateur peut continuer à accéder aux dossiers publics à l’aide d’OWA ou d’Outlook pour Mac.</span><span class="sxs-lookup"><span data-stu-id="06c7e-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="06c7e-118">Pour plus d’informations, consultez la rubrique [annonce de la prise en charge des connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="06c7e-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>