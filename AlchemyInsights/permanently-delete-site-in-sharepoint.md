---
title: Supprimer définitivement un site dans SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771719"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Supprimer définitivement un site dans SharePoint

Pour réutiliser une URL à partir d’un site supprimé (pour recréer un site) ou pour supprimer définitivement un site, car il n’est plus utilisé, vous pouvez utiliser **Supprimer définitivement** du nouveau centre d’administration SharePoint. 

1. Accédez à la [Page de sites supprimées du nouveau Centre d’administration SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) et connectez-vous à l’aide d’un compte disposant des autorisations d’administrateur pour votre organisation. 

2. Dans la colonne de gauche, sélectionnez un site. 

3. Cliquez sur **supprimer définitivement**. 

**Remarque**: les sites connectés au groupe ne peuvent pas être supprimés définitivement du nouveau centre d’administration SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) devra être utilisé à la place.  

Pour plus d'informations, consultez la rubrique [Suppression définitive d’un site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
