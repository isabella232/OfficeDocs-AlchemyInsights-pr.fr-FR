---
title: Les messages envoyés au groupe Microsoft 365 ne sont pas reçus par tous les membres
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976503"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Les messages envoyés à un groupe Microsoft 365 ne sont pas reçus par tous les membres

Veuillez à ce que tous les membres du groupe soient abonnés pour recevoir les e-mails. Voir [Suivre un groupe dans Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Pour vérifier l’état des messages des membres qui se sont abonnés aux e-mails de groupe, exécutez la commande suivante sur [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) :

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Utilisez la commande PowerShell EXO pour configurer tous les membres du groupe de manière à ce qu’ils reçoivent les messages envoyés à un groupe Microsoft 365 dans leur boîte de réception :

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Par exemple :

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`