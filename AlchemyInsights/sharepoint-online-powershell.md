---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830580"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Vous travaillez avec PowerShell ou des scripts dans Sharepoint Online ? Pour plus d'informations, consultez les liens ci-dessous.
- [Prise en main de SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Se connecter à SPO PowerShell avec l'authentification multifacteur (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Les modèles et pratiques [SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contiennent une bibliothèque de commandes PowerShell qui vous permet d'effectuer des actions de gestion complexes vers SPO.

> [!NOTE]
> - Si vous avez des problèmes de connexion avec l'environnement de ligne de commande SPO Management Shell, assurez-vous que vous avez mis à jour la dernière version et essayez de [ré-importer](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) le module à l'aide de « *Import-Module Microsoft.Online.SharePoint.PowerShell ».*
> - Si vous tentez d'exécuter des scripts de modèle objet côté client, vous devez avoir installé le [SDK Composants](https://www.microsoft.com/download/details.aspx?id=42038) client Sharepoint Online sur votre ordinateur local.
> - Si vous avez des problèmes lors de l'exécution de scripts à partir de PowerShell, vous pouvez envisager d'exécuter PowerShell en tant qu'administrateur et de modifier la stratégie [d'exécution.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)