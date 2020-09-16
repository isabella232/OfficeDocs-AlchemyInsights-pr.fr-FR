---
title: Chiffrement avec les règles de transport
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784341"
---
# <a name="encryption-with-transport-rules"></a>Chiffrement avec les règles de transport

Dans le [Centre d’administration Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (CAE), vous pouvez utiliser les fonctionnalités de chiffrement de messages Office (OME) dans vos règles de flux de courrier pour déclencher le chiffrement des messages. Sélectionnez l’option **Appliquer le chiffrement de messages Office 365 et la protection des droits** dans la condition de règle de transport.

- Pour plus d’informations, consultez l’article [Définir une règle de flux de courrier pour chiffrer](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Dans PowerShell, utilisez l’applet de commande [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) et attribuez au paramètre *ApplyOME* la valeur $true.
