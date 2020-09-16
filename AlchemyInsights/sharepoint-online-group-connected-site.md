---
title: Ajouter un groupe à un site SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771198"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problèmes lors de la création d’un site connecté à un groupe dans SharePoint

1. Certains problèmes courants lors de la création ou de la recréation d’un site connecté à un groupe.
Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.

   - Télécharger [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Pour plus d’informations sur la prise en main de PowerShell, voir [Getting Started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Supprimez le site des sites supprimés à l’aide de l’applet de commande PowerShell [Remove-spodeletedsit](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell est nécessaire pour supprimer définitivement les sites de groupe.

1. Si vous créez un site connecté à un groupe et recevez un avertissement : **un autre groupe avec le même alias existe déjà**, vérifiez les groupes existants à partir du [Centre d’administration Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez-en un autre.

1. Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.

   - Vous pouvez connecter des sites existants à un groupe Microsoft 365. Pour plus d’informations, consultez [la rubrique Connect a Microsoft 365 Group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Pour créer un site connecté à un groupe Microsoft 365, vous devez créer un [site d’équipe](https://admin.microsoft.com/sharepoint).
