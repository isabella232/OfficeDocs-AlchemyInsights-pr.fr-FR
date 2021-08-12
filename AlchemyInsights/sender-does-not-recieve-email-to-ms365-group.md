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
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958295"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>L’expéditeur ne reçoit pas le courrier envoyé au groupe Microsoft 365

Par défaut, l’expéditeur d’un message électronique envoyé à un groupe Microsoft 365 ne reçoit pas de copie du message dans sa boîte de réception, même s’il est membre du groupe.

Utilisez cette commande PowerShell EXO pour autoriser l’expéditeur à recevoir une copie de chaque message qu’il envoie au groupe Microsoft 365 :  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Pour activer le paramètre pour toutes les boîtes aux lettres à la fois :

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Remarque** Une heure peut s’écouler avant que les modifications apportées à ce paramètre prennent effet.