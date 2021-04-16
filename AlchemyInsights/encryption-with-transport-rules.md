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
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813866"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="8c3cb-102">Chiffrement avec les règles de transport</span><span class="sxs-lookup"><span data-stu-id="8c3cb-102">Encryption with transport rules</span></span>

<span data-ttu-id="8c3cb-103">Dans le [Centre d’administration Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (CAE), vous pouvez utiliser les fonctionnalités de chiffrement de messages Office (OME) dans vos règles de flux de courrier pour déclencher le chiffrement des messages.</span><span class="sxs-lookup"><span data-stu-id="8c3cb-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="8c3cb-104">Sélectionnez l’option **Appliquer le chiffrement de messages Office 365 et la protection des droits** dans la condition de règle de transport.</span><span class="sxs-lookup"><span data-stu-id="8c3cb-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="8c3cb-105">Pour plus d’informations, consultez l’article [Définir une règle de flux de courrier pour chiffrer](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="8c3cb-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="8c3cb-106">Dans PowerShell, utilisez l’applet de commande [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) et attribuez au paramètre *ApplyOME* la valeur $true.</span><span class="sxs-lookup"><span data-stu-id="8c3cb-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
