---
title: 2419-impossible d’activer-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767597"
---
# <a name="unable-to-enable-unified-auditing"></a>Impossible d’activer l’audit unifié

Lorsque vous essayez d’activer l’audit unifié pour votre organisation, il se peut que vous receviez une erreur similaire à celle-ci :

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Pour résoudre ce problème, procédez comme suit :

1. [Connectez-vous à Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Exécutez la cmdlet suivante :

   ```
   Enable-OrganizationCustomization
   ```

3. Attendez 60 minutes que le paramètre précédent prenne effet.

4. Exécutez la commande suivante dans Exchange Online PowerShell :

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Pour plus d’informations, consultez les articles suivants :

- [Connexion à Exchange Online PowerShell avec l’authentification multifacteur](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activer ou désactiver la recherche dans le journal d’audit](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
