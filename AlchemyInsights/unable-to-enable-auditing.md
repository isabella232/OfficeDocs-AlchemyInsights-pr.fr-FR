---
title: 2419 -unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007788"
---
# <a name="unable-to-enable-unified-auditing"></a>Impossible d’activer l’audit unifié

Lorsque vous essayez d’activer l’audit unifié pour votre organisation, vous pouvez recevoir une erreur semblable à celle-ci :

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Pour résoudre ce problème, suivez les étapes suivantes :

1. [Connecter à Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Exécutez la l’applet commande suivant :

   ```
   Enable-OrganizationCustomization
   ```

3. Patientez 60 minutes avant que le paramètre précédent prenne effet.

4. Exécutez la commande suivante dans Exchange Online PowerShell :

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Pour plus d’informations, voir les articles suivants :

- [Connexion à Exchange Online PowerShell avec l’authentification multifacteur](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activer ou désactiver la recherche dans les journaux d'audit](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
