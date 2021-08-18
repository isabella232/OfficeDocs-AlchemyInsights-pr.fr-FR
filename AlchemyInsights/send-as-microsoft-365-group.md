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
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086126"
---
# <a name="send-as-microsoft-365-group"></a>Envoyer en tant que groupe Microsoft 365

Vous pouvez attribuer des autorisations Envoyer en tant que pour permettre à des utilisateurs spécifiques d’envoyer des messages en tant que groupe Microsoft 365 :  

1. Connectez-vous à Exchange Online PowerShell.  

2. Exécutez la commande suivante :  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -Trustee AccessRights

Si vous souhaitez obtenir plus d’informations, voir [Autoriser les membres à envoyer en tant que ou de la part d'un groupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).