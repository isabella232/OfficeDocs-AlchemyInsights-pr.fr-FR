---
title: Problèmes de performances-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068398"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive est lent, inaccessible ou indisponible pour plusieurs utilisateurs

SharePoint ou OneDrive sont peut-être lents, inaccessibles ou indisponibles, ou peuvent afficher le service non disponible ou des erreurs 503, pour plusieurs raisons :
  
- Si votre site SharePoint ou OneDrive est lent ou retardé pour plusieurs utilisateurs, il peut y avoir un problème de service temporaire dans lequel les utilisateurs subissent des retards ou des erreurs de navigation intermittents lors de l’accès à des sites SharePoint ou à du contenu OneDrive. Consultez le [tableau de bord d’État du service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour voir si votre organisation est concernée.
  
- Les utilisateurs peuvent recevoir un message d’erreur « le *serveur 503 est occupé* » lors de la tentative de navigation vers des sites SharePoint ou OneDrive. Cette erreur peut être causée par la limitation dans le service SharePoint. SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online. Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources. Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Si vous constatez un ralentissement des performances avec un site ou une page SharePoint **classique** ou **moderne** , utilisez l' [outil de diagnostic de page](https://aka.ms/perftool) pour analyser les pages.
  
- Si les performances générales sont toujours déchargées, consultez les ressources au bas de cet article : [Présentation de l’optimisation des performances pour SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  