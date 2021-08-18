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
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320354"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Définir ClientAccessServerEnabled sur True

Si vous ne pouvez pas ouvrir un message électronique chiffré et voir une pièce jointe **rpmsg,** effectuez les étapes suivantes :

1. Connectez-vous à Exchange Online PowerShell.

    **Remarque**: pour vous connecter à Exchange Online PowerShell, vous devez vous connecter à l’aide d’un compte d’administrateur global ou Exchange administrateur.

   a. Ouvrez Windows PowerShell, puis exécutez la commande suivante :`$UserCredential = Get-Credential`
   b. Dans la **boîte Windows PowerShell demande d’informations** d’identification, entrez votre compte et mot de passe scolaire ou scolaire, c. Cliquez sur **OK**. 

2. Exécutez la commande suivante pour créer une session :

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Exécutez la commande suivante :
    
    `Import-PSSession $Session -DisableNameChecking`

3. Exécutez `Get-IRMConfiguration` la commande.

4. Vérifiez le **paramètre ClientAccessServerEnabled.** 

    a. Si **le paramètre ClientAccessServerEnabled** est définie sur **False,** exécutez l’cmdlet suivante : `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Conseil**: fermez toujours votre session PowerShell avec la commande suivante : `Remove-PSSession $Session`

Pour plus d’informations, [voir Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

