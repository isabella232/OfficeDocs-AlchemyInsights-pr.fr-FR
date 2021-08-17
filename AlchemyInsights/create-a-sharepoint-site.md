---
title: Créer un site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080888"
---
# <a name="create-a-sharepoint-site"></a>Créer un site SharePoint

Créez ou gérez des sites à [partir de Sites actifs](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) dans SharePoint Admin Center. Pour plus d’informations, voir [Gérer les sites dans le nouveau centre SharePoint’administration.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>Astuces :

- Vous **ne** pouvez pas créer un site avec la même URL qu’un site existant. Si vous avez supprimé un site et que vous souhaitez ré-utiliser l’URL, il est possible que le site supprimé existe toujours sous [Sites supprimés.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) Le site doit être définitivement supprimé pour pouvoir utiliser à nouveau l’URL. Pour supprimer complètement un site avec PowerShell, voir l’exemple d’cmdlet [Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- Certains utilisateurs peuvent ne pas être en mesure de créer un site. [Voir Gérer la création de sites dans SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)
- Il est possible que le site apparaisse bloqué au niveau **Création** plus longtemps que prévu. Si plus de 24 heures se sont écoulées depuis le premier problème, veuillez enregistrer un ticket de support. Dans de nombreux cas, nous travaillons déjà sur une solution. Veuillez nous donner au moins 24 heures pour terminer une solution.
