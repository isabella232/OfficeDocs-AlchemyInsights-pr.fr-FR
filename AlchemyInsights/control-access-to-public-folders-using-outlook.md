---
title: Contrôler l’accès aux dossiers publics à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406561"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="fe59a-102">Contrôler l’accès aux dossiers publics à l’aide d’Outlook</span><span class="sxs-lookup"><span data-stu-id="fe59a-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="fe59a-103">Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook :</span><span class="sxs-lookup"><span data-stu-id="fe59a-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="fe59a-104">Utiliser `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="fe59a-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="fe59a-105">$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook</span><span class="sxs-lookup"><span data-stu-id="fe59a-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="fe59a-106">$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook.</span><span class="sxs-lookup"><span data-stu-id="fe59a-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="fe59a-107">Ceci est la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="fe59a-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="fe59a-108">Remarque : Cette procédure peut uniquement contrôler les connexions avec les applications de bureau Outlook pour les clients Windows.</span><span class="sxs-lookup"><span data-stu-id="fe59a-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="fe59a-109">Les utilisateurs ont toujours accès aux dossiers publics par le biais d’OWA ou d’Outlook pour Mac.</span><span class="sxs-lookup"><span data-stu-id="fe59a-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="fe59a-110">Pour plus d’informations, se référer à la rubrique [Connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="fe59a-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
