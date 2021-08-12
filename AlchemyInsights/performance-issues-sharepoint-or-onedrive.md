---
title: 'Problèmes de performances : SharePoint ou OneDrive'
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911840"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lent, inaccessible ou indisponible pour plusieurs utilisateurs

SharePoint ou OneDrive peuvent être lentes, inaccessibles ou indisponibles, ou afficher des erreurs de service indisponibles ou 503, pour plusieurs raisons :
  
- Si votre site SharePoint ou OneDrive est lent ou retardé pour plusieurs utilisateurs, il peut y avoir un problème de service temporaire dans lequel les utilisateurs rencontrent des retards intermittents ou des erreurs de navigation lors de l’accès à des sites SharePoint ou à OneDrive contenu. Consultez le [Tableau de bord d’intégrité du service ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour déterminer si votre organisation est affectée.
  
- Les utilisateurs peuvent recevoir une erreur de occupé du serveur *503* lorsque vous tentez d’accéder à SharePoint ou OneDrive sites. Cette erreur peut être causée par la limitation au sein du service SharePoint service. SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online. Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources. Pour plus d’informations sur la limitation, évitez d’être limitée [ou bloquée dans SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Si les performances sont  lentes avec un site ou une page SharePoint classique ou moderne, utilisez l’outil [Diagnostic](https://aka.ms/perftool) de page pour analyser les pages. 
  
- Si les performances générales sont toujours lentes, consultez les ressources au bas de cet article : Introduction à l’optimisation des performances [pour SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  