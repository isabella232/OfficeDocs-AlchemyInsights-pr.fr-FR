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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070296"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utiliser Exchange Online PowerShell pour activer DKIM pour un domaine spécifique

Si vous ne pouvez pas créer les enregistrements DKIM DNS dans le Centre d’administration, essayez d’Exchange Online PowerShell. 

Pour créer un enregistrement DNS DKIM à l’Exchange Online PowerShell, effectuez les étapes suivantes :

1. Ouvrez Windows PowerShell en tant qu’administrateur et exécutez les commandes suivantes dans la séquence décrite :

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Si vous avez des difficultés à vous connecter Exchange Online PowerShell, consultez Connecter [à Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Une fois que vous êtes connecté à Exchange Online PowerShell, exécutez la commande suivante :

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Une fois que la commande ci-dessus a été exécutée avec succès, exécutez la commande suivante pour mettre fin à Exchange Online session PowerShell suivante :

    `Remove-PSSession $Session` 



