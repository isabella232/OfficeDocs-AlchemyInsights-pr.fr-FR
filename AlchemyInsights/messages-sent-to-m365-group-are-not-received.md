---
title: Les messages envoyés au groupe Microsoft 365 ne sont pas reçus par tous les membres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: fr-FR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45047233"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Les messages envoyés à un groupe Microsoft 365 ne sont pas reçus par tous les membres

Assurez-vous que tous les membres du groupe se sont abonnés pour recevoir les e-mails. Voir [Suivre un groupe dans Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Pour vérifier l’état des messages des membres qui se sont abonnés aux e-mails de groupe, exécutez la commande suivante sur [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps) :

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`