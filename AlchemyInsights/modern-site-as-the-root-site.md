---
title: Site moderne comme site racine
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057707"
---
# <a name="modern-site-as-root-site"></a>Site moderne en tant que site racine

Les clients disposant de la [version cible](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) peuvent désormais activer l’expérience de site de communication moderne sur le site racine classique de leur client SharePoint.

Cette fonctionnalité peut être activée en exécutant une cmdlet PowerShell simple. Lors de l’exécution réussie de la ou des commandes PowerShell, le site racine aura une nouvelle page d’accueil de site de communication. Pour plus d’informations sur les applets de commande et les fonctionnalités de PowerShell, consultez l’article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Nous effectuerons progressivement cette opération, désactivée par défaut, pour les clients ciblés dans le premier mai 2019, et le déploiement sera disponible dans le monde entier à la fin du 2019 juin. Continuez à vous référer au [Centre de messages](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) pour les autres nouvelles fonctionnalités de moderne. 

**Important**: ne supprimez pas votre site racine classique pour créer un site de communication moderne. Ceci n’est pas pris en charge par Microsoft. La suppression du site racine rendra tous les sites SharePoint de votre organisation inaccessibles à tous les utilisateurs, jusqu’à ce que vous restauriez le site ou que vous créez un nouveau site à la même URL. 
 
 