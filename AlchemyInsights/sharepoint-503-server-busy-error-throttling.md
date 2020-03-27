---
title: Limitation de SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958717"
---
# <a name="sharepoint-online-throttling"></a>Limitation de SharePoint Online

**Important**: pendant ces temps inégalés, nous faisons en sorte de s’assurer que les services SharePoint Online et OneDrive restent hautement disponibles : consultez les [ajustements de fonctionnalité temporaire SharePoint Online](https://aka.ms/ODSPAdjustments) pour plus d’informations.

**erreur de disponibilité du serveur 503**

Les utilisateurs peuvent recevoir un message d’erreur « le serveur 503 est occupé » lors de la tentative de navigation vers des sites SharePoint ou OneDrive. 

Cette erreur peut être causée par la limitation dans le service SharePoint. SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online. Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources. 

Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Si vous pensez que cette erreur n’est pas liée à la limitation, vous pouvez vérifier si la maintenance active a lieu sur votre client en accédant au [Centre de messages](https://portal.office.com/adminportal/home#/MessageCenter).

 Enfin, vous devez consulter la page [État du service](https://portal.office.com/adminportal/home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire.

