---
title: Envoyer en tant que groupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740149"
---
# <a name="send-as-microsoft-365-group"></a>Envoyer en tant que groupe Microsoft 365

Vous pouvez attribuer des autorisations Envoyer en tant que pour permettre à des utilisateurs spécifiques d’envoyer des messages en tant que groupe Microsoft 365 :  

1. Connectez-vous à Exchange Online PowerShell.  

2. Exécutez la commande suivante :  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -Trustee AccessRights

Si vous souhaitez obtenir plus d’informations, voir [Autoriser les membres à envoyer en tant que ou de la part d'un groupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).