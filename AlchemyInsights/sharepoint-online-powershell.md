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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="be3d4-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="be3d4-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="be3d4-103">Vous utilisez PowerShell ou des scripts dans SharePoint Online ?</span><span class="sxs-lookup"><span data-stu-id="be3d4-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="be3d4-104">Pour plus d’informations, consultez les liens ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="be3d4-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="be3d4-105">Prise en main de SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="be3d4-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="be3d4-106">Se connecter à SPO PowerShell avec l’authentification multifacteur (MFA)</span><span class="sxs-lookup"><span data-stu-id="be3d4-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="be3d4-107">[SharePoint Patterns and Practices (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contient une bibliothèque de commandes PowerShell qui vous permet d’effectuer des actions de gestion complexes vers SPO.</span><span class="sxs-lookup"><span data-stu-id="be3d4-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="be3d4-108">Si vous rencontrez des problèmes lors de la connexion avec l’environnement de ligne de commande SPO Management Shell, vérifiez que vous avez mis à jour vers la dernière version et essayez de [réimporter le module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) à l’aide du *"import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="be3d4-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="be3d4-109">Si vous tentez d’exécuter des scripts de modèle objet côté client, le [Kit de développement logiciel (SDK) des composants clients SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) doit être installé sur votre ordinateur local.</span><span class="sxs-lookup"><span data-stu-id="be3d4-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="be3d4-110">Si vous rencontrez des problèmes lors de l’exécution de scripts à partir de PowerShell, vous pouvez envisager d’exécuter PowerShell en tant qu’administrateur et de modifier la [stratégie d’exécution](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="be3d4-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>