---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770837"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Vous utilisez PowerShell ou des scripts dans SharePoint Online ? Pour plus d’informations, consultez les liens ci-dessous.
- [Prise en main de SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Se connecter à SPO PowerShell avec l’authentification multifacteur (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contient une bibliothèque de commandes PowerShell qui vous permet d’effectuer des actions de gestion complexes vers SPO.

> [!NOTE]
> - Si vous rencontrez des problèmes lors de la connexion avec l’environnement de ligne de commande SPO Management Shell, vérifiez que vous avez mis à jour vers la dernière version et essayez de [réimporter le module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) à l’aide du *"import-module Microsoft. online. SharePoint. PowerShell".*
> - Si vous tentez d’exécuter des scripts de modèle objet côté client, le [Kit de développement logiciel (SDK) des composants clients SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) doit être installé sur votre ordinateur local.
> - Si vous rencontrez des problèmes lors de l’exécution de scripts à partir de PowerShell, vous pouvez envisager d’exécuter PowerShell en tant qu’administrateur et de modifier la [stratégie d’exécution](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).