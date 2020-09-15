---
title: Contrôler l’accès aux dossiers publics à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680484"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="280c2-102">Contrôler l’accès aux dossiers publics à l’aide d’Outlook</span><span class="sxs-lookup"><span data-stu-id="280c2-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="280c2-103">Pour contrôler quels utilisateurs peuvent accéder aux dossiers publics à l’aide d’Outlook :</span><span class="sxs-lookup"><span data-stu-id="280c2-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="280c2-104">Utiliser `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="280c2-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="280c2-105">$true : Autoriser l’accès des utilisateurs aux dossiers publics dans Outlook</span><span class="sxs-lookup"><span data-stu-id="280c2-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="280c2-106">$false : Empêcher l’accès des utilisateurs aux dossiers publics dans Outlook.</span><span class="sxs-lookup"><span data-stu-id="280c2-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="280c2-107">Ceci est la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="280c2-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="280c2-108">Remarque : Cette procédure peut uniquement contrôler les connexions avec les applications de bureau Outlook pour les clients Windows.</span><span class="sxs-lookup"><span data-stu-id="280c2-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="280c2-109">Les utilisateurs ont toujours accès aux dossiers publics par le biais d’OWA ou d’Outlook pour Mac.</span><span class="sxs-lookup"><span data-stu-id="280c2-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="280c2-110">Pour plus d’informations, se référer à la rubrique [Connexions contrôlées aux dossiers publics dans Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="280c2-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
