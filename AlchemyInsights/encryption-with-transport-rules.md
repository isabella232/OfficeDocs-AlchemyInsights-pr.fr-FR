---
title: Chiffrement avec les règles de transport
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079448"
---
# <a name="encryption-with-transport-rules"></a>Chiffrement avec les règles de transport

Dans le [Centre d’administration Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (CAE), vous pouvez utiliser les fonctionnalités de chiffrement de messages Office (OME) dans vos règles de flux de courrier pour déclencher le chiffrement des messages. Sélectionnez l’option **Appliquer le chiffrement de messages Office 365 et la protection des droits** dans la condition de règle de transport.

- Pour plus d’informations, consultez l’article [Définir une règle de flux de courrier pour chiffrer](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Dans PowerShell, utilisez l’applet de commande [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) et attribuez au paramètre *ApplyOME* la valeur $true.
