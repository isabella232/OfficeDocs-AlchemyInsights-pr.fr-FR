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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719480"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Créer un site connecté à un groupe dans SharePoint Online

<p><strong>Il existe deux problèmes courants lors de la création ou de la recréation d’un site connecté à un groupe.&nbsp;</strong></p>  <p>1.Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.</p>  <ul>  <li>Télécharger <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - pour plus d’informations sur la prise en main de <a title="PowerShell, voir Getting Started with SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Prise en main de SharePoint Online Management</a>Shell. <br /><br /></li>  <li>Supprimer le site des sites supprimés à l' <a title="aide de la spodeletedsit" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Suppression de l'</a> applet de commande PowerShell spodeletedsit.</li>  </ul>  <p>Si vous créez un site de groupe connecté et que vous recevez un message d’avertissement <strong>«un autre groupe avec le même alias existe déjà»</strong>, vérifiez <a title="les groupes existants à partir du centre d’administration de Microsoft Office 365" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 à partir du centre</a>d’administration. Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez-en un autre.&nbsp;</p>  <p><strong>Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.&nbsp;</strong></p>  <ol>  <li>Vous pouvez connecter des sites existants à un groupe Office 365. Pour plus d’informations, <a title="consultez la rubrique Connect an Office 365 Group using the SharePoint User ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Connectez un groupe Office 365 à l’aide de l'</a>utilisateur SharePoint ineterface.</li>  <li>Pour créer un site connecté à un groupe Office 365, vous devez créer un site d’équipe. Pour plus d’informations, <a title="consultez la rubrique créer un site d’équipe dans SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Créez un site d’équipe dans SharePoint.</a></li>  </ol>

