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
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318122"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problèmes courants lors de la création d’un site connecté à un groupe dans SharePoint

1. Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.

   - Télécharger [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Pour plus d’informations sur la prise en charge de PowerShell, voir Prise en SharePoint [Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Supprimez le site des sites supprimés à l’aide de la cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell est nécessaire pour supprimer définitivement les sites de groupe.

1. Si vous créez un site connecté à un groupe et recevez un avertissement : un autre groupe avec le même **alias** existe déjà, vérifiez les groupes existants à partir du [Centre d’administration Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez le site avec un autre alias attribué.

1. Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.

   - Vous pouvez connecter des sites existants à un Microsoft 365 groupe. Pour plus d’informations, [Connecter un groupe Microsoft 365 à l’aide de l SharePoint’interface utilisateur.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Pour créer un site Microsoft 365 de groupe, vous devez créer un [site d’équipe.](https://admin.microsoft.com/sharepoint)
