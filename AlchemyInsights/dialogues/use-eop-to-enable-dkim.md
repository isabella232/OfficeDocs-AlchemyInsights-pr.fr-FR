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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utiliser Exchange Online PowerShell pour activer DKIM pour un domaine spécifique

Si vous ne pouvez pas créer les enregistrements DKIM DNS dans le centre d’administration, essayez d’utiliser Exchange Online PowerShell. 

Pour créer un enregistrement DNS DKIM à l’aide d’Exchange Online PowerShell, effectuez les étapes suivantes :

1. Ouvrez Windows PowerShell en tant qu’administrateur et exécutez les commandes suivantes dans la séquence décrite :

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Si vous avez des difficultés pour vous connecter à Exchange Online PowerShell, consultez La connexion [à Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Une fois connecté à Exchange Online PowerShell, exécutez la commande suivante :

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Une fois que la commande ci-dessus a été exécutée avec succès, exécutez la commande suivante pour mettre fin à la session Exchange Online PowerShell :

    `Remove-PSSession $Session` 



