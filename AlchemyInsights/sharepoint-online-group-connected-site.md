---
title: Ajouter un groupe à un site SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758729"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Créer un site connecté à un groupe dans SharePoint Online

Il existe deux problèmes courants lors de la création ou de la recréation d’un site connecté à un groupe.

 Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.

Télécharger [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Pour plus d’informations sur la prise en main de PowerShell, voir [Getting Started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Supprimez le site des sites supprimés à l’aide de l’applet de commande PowerShell [Remove-spodeletedsit](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Si vous créez un site de groupe connecté et que vous recevez un avertissement, un autre groupe avec le même alias existe déjà, vérifiez les groupes existants à partir du [Centre d’administration Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez-en un autre.

Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.

Vous pouvez connecter des sites existants à un groupe Office 365. Pour plus d’informations, consultez [la rubrique Connect an Office 365 Group using the SharePoint User ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Pour créer un site connecté à un groupe Office 365, vous devez créer un site d’équipe. Pour plus d’informations, consultez [la rubrique créer un site d’équipe dans SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).
