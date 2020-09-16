---
title: Problèmes de performances-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771899"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive est lent, inaccessible ou indisponible pour plusieurs utilisateurs

SharePoint ou OneDrive sont peut-être lents, inaccessibles ou indisponibles, ou peuvent afficher le service non disponible ou des erreurs 503, pour plusieurs raisons :
  
- Si votre site SharePoint ou OneDrive est lent ou retardé pour plusieurs utilisateurs, il peut y avoir un problème de service temporaire dans lequel les utilisateurs subissent des retards ou des erreurs de navigation intermittents lors de l’accès à des sites SharePoint ou à du contenu OneDrive. Consultez le [Tableau de bord d’intégrité du service ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour déterminer si votre organisation est affectée.
  
- Les utilisateurs peuvent recevoir un message d’erreur « le *serveur 503 est occupé* » lors de la tentative de navigation vers des sites SharePoint ou OneDrive. Cette erreur peut être causée par la limitation dans le service SharePoint. SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online. Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources. Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Si vous constatez un ralentissement des performances avec un site ou une page SharePoint **classique** ou **moderne** , utilisez l' [outil de diagnostic de page](https://aka.ms/perftool) pour analyser les pages.
  
- Si les performances générales sont toujours déchargées, consultez les ressources au bas de cet article : [Présentation de l’optimisation des performances pour SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  