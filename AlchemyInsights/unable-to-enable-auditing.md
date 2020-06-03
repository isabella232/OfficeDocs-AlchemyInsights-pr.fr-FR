---
title: 2419-impossible d’activer-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510426"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="ac972-102">Impossible d’activer l’audit unifié</span><span class="sxs-lookup"><span data-stu-id="ac972-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="ac972-103">Lorsque vous essayez d’activer l’audit unifié pour votre organisation, il se peut que vous receviez une erreur similaire à celle-ci :</span><span class="sxs-lookup"><span data-stu-id="ac972-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="ac972-104">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ac972-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="ac972-105">[Connectez-vous à Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="ac972-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="ac972-106">Exécutez la cmdlet suivante :</span><span class="sxs-lookup"><span data-stu-id="ac972-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="ac972-107">Attendez 60 minutes que le paramètre précédent prenne effet.</span><span class="sxs-lookup"><span data-stu-id="ac972-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="ac972-108">Exécutez la commande suivante dans Exchange Online PowerShell :</span><span class="sxs-lookup"><span data-stu-id="ac972-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="ac972-109">Pour plus d’informations, consultez les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="ac972-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="ac972-110">Connexion à Exchange Online PowerShell avec l’authentification multifacteur</span><span class="sxs-lookup"><span data-stu-id="ac972-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="ac972-111">Activer ou désactiver la recherche dans le journal d’audit</span><span class="sxs-lookup"><span data-stu-id="ac972-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
