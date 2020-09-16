---
title: 'MC210173 : l’obsolescence de la nouvelle fonctionnalité de formulaire personnalisé de SharePoint Designer'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: a53b8885a877cb688cfb42bb4f9108cb2cef2418
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743809"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 : l’obsolescence de la nouvelle fonctionnalité de formulaire personnalisé de SharePoint Designer

Nous avons identifié un problème affectant les fonctionnalités de SharePoint Designer pour [création de formulaires personnalisés](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) dans SharePoint Online. Après un examen minutieux, nous avons déterminé qu'il n'y a pas de solution connue pour résoudre ce problème et nous avons choisi de désactiver la fonction de création de formulaires personnalisés à partir de 3h00 UTC le samedi 25 avril 2020. Cette modification n’affecte pas la possibilité de modifier des formulaires déjà créés ou d’autres fonctionnalités existantes dans le concepteur SharePoint Online.

Une fois cette modification apportée, les utilisateurs peuvent avoir reçu l’erreur : « Impossible d’enregistrer les modifications apportées à la liste sur le serveur » lors de la création de formulaires.

Les utilisateurs qui ont déjà exploité SharePoint Designer pour créer des formulaires personnalisés peuvent plutôt utiliser [PowerApp](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) à cet effet.

PowerApps est un outil simple et puissant qui permet aux utilisateurs d’utiliser l’expérience moderne de SharePoint Online pour créer et modifier des formulaires personnalisés pour des listes et des bibliothèques de documents SharePoint directement à partir d’une fenêtre de navigateur. Les applications PowerApp n’ont pas besoin de connaissances de codage classiques ou de téléchargements d’applications supplémentaires tels qu’InfoPath.

**Remarque** : les utilisateurs de SharePoint Online Classic devront basculer temporairement vers l’expérience moderne pour accéder et utiliser PowerApps. Cependant, tous les formulaires personnalisés créés dans PowerApp sont accessibles aux utilisateurs de l’expérience classique de SharePoint Online.
