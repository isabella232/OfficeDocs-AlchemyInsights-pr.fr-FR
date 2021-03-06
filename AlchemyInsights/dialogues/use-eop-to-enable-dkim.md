---
title: Utiliser Exchange Online PowerShell pour activer DKIM pour un domaine spécifique
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500739"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="76d95-102">Utiliser Exchange Online PowerShell pour activer DKIM pour un domaine spécifique</span><span class="sxs-lookup"><span data-stu-id="76d95-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="76d95-103">Si vous ne pouvez pas créer les enregistrements DKIM DNS dans le centre d’administration, essayez d’utiliser Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="76d95-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="76d95-104">Pour créer un enregistrement DNS DKIM à l’aide d’Exchange Online PowerShell, effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="76d95-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="76d95-105">Ouvrez Windows PowerShell en tant qu’administrateur et exécutez les commandes suivantes dans la séquence décrite :</span><span class="sxs-lookup"><span data-stu-id="76d95-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="76d95-106">a.</span><span class="sxs-lookup"><span data-stu-id="76d95-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="76d95-107">b.</span><span class="sxs-lookup"><span data-stu-id="76d95-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="76d95-108">c.</span><span class="sxs-lookup"><span data-stu-id="76d95-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="76d95-109">Si vous avez des difficultés pour vous connecter à Exchange Online PowerShell, consultez La connexion [à Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="76d95-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="76d95-110">Une fois connecté à Exchange Online PowerShell, exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="76d95-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="76d95-111">Une fois que la commande ci-dessus a été exécutée avec succès, exécutez la commande suivante pour mettre fin à la session Exchange Online PowerShell :</span><span class="sxs-lookup"><span data-stu-id="76d95-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



