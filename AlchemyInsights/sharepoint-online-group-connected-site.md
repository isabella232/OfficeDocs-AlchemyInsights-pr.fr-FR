---
title: Ajouter un groupe à un site SharePoint site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 396efbf9772b5398427a4fcc76e104fa95820af6
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532217"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problèmes courants lors de la création d’un site connecté à un groupe dans SharePoint

1. Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.

   - Télécharger [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Pour plus d’informations sur la prise en charge de PowerShell, voir Prise en SharePoint [Online Management Shell.](/powershell/module/sharepoint-online/remove-sposite)
   - Supprimez le site des sites supprimés à l’aide de l’cmdlet [Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell est nécessaire pour supprimer définitivement les sites de groupe.

1. Si vous créez un site connecté à un groupe et recevez un avertissement : un autre groupe avec le même **alias** existe déjà, vérifiez les groupes existants à partir du [Centre d’administration Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez le site avec un autre alias attribué.

1. Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.

   - Vous pouvez connecter des sites existants à un Microsoft 365 groupe. Pour plus d’informations, [Connecter un groupe Microsoft 365 à l’aide de l SharePoint’interface utilisateur.](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Pour créer un site Microsoft 365 de groupe, vous devez créer un [site d’équipe.](https://admin.microsoft.com/sharepoint)
