---
title: Définir ClientAccessServerEnabled sur True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509748"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="5ad7e-102">Définir ClientAccessServerEnabled sur True</span><span class="sxs-lookup"><span data-stu-id="5ad7e-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="5ad7e-103">Si vous ne pouvez pas ouvrir un message électronique chiffré et voir une pièce jointe **rpmsg,** effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="5ad7e-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="5ad7e-104">Connectez-vous à Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="5ad7e-105">Pour vous connecter à Exchange Online PowerShell, vous devez vous connecter à l’aide d’un compte d’administrateur global ou d’administrateur Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="5ad7e-106">a.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-106">a.</span></span> <span data-ttu-id="5ad7e-107">Ouvrez Windows PowerShell, puis exécutez la commande suivante : `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="5ad7e-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="5ad7e-108">b.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-108">b.</span></span> <span data-ttu-id="5ad7e-109">Dans la **boîte Windows PowerShell demande d’informations** d’identification, entrez votre compte et mot de passe scolaire ou scolaire, c.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="5ad7e-110">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-110">Click **OK**.</span></span> 

2. <span data-ttu-id="5ad7e-111">Exécutez la commande suivante pour créer une session :</span><span class="sxs-lookup"><span data-stu-id="5ad7e-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="5ad7e-112">a.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-112">a.</span></span> <span data-ttu-id="5ad7e-113">Exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="5ad7e-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="5ad7e-114">Exécutez `Get-IRMConfiguration` la commande.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="5ad7e-115">Vérifiez le **paramètre ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="5ad7e-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="5ad7e-116">a.</span><span class="sxs-lookup"><span data-stu-id="5ad7e-116">a.</span></span> <span data-ttu-id="5ad7e-117">Si **le paramètre ClientAccessServerEnabled** est définie sur **False,** exécutez l’cmdlet suivante : `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="5ad7e-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="5ad7e-118">Fermez toujours votre session PowerShell avec la commande suivante : `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="5ad7e-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="5ad7e-119">Pour plus d’informations, [voir Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="5ad7e-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

