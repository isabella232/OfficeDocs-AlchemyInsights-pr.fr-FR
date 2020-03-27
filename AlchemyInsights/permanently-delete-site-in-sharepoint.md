---
title: Supprimer définitivement un site dans SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955172"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Supprimer définitivement un site dans SharePoint

Pour réutiliser une URL à partir d’un site supprimé (pour recréer un site) ou pour supprimer définitivement un site, car il n’est plus utilisé, vous pouvez utiliser **Supprimer définitivement** du nouveau centre d’administration SharePoint. 

1. Accédez à la [Page de sites supprimées du nouveau Centre d’administration SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) et connectez-vous à l’aide d’un compte disposant des autorisations d’administrateur pour votre organisation. 

2. Dans la colonne de gauche, sélectionnez un site. 

3. Cliquez sur **supprimer définitivement**. 

**Remarque**: les sites connectés au groupe ne peuvent pas être supprimés définitivement du nouveau centre d’administration SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) devra être utilisé à la place.  

Pour plus d'informations, consultez la rubrique [Suppression définitive d’un site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
