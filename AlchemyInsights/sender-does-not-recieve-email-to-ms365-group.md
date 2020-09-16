---
title: L’expéditeur ne reçoit pas le courrier envoyé au groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751313"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>L’expéditeur ne reçoit pas le courrier envoyé au groupe Microsoft 365

Par défaut, l’expéditeur d’un message électronique envoyé à un groupe Microsoft 365 ne reçoit pas de copie du message dans sa boîte de réception, même s’il est membre du groupe.

Utilisez cette commande PowerShell EXO pour autoriser l’expéditeur à recevoir une copie de chaque message qu’il envoie au groupe Microsoft 365 :  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Pour activer le paramètre pour toutes les boîtes aux lettres à la fois :

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Remarque** Une heure peut s’écouler avant que les modifications apportées à ce paramètre prennent effet.