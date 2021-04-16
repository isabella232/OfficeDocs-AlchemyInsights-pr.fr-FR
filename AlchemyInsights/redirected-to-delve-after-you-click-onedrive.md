---
title: OneDrive Entreprise Web OneDrive redirige vers Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799987"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirigé vers Delve après avoir cliqué sur OneDrive

Consultez notre guide [de dépannage détaillé.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Pour résoudre ce problème, l'administrateur doit accorder aux utilisateurs le droit de créer leur site Mes sites. Cela est dû au fait que la page OneDrive Entreprise est créée sur Mes sites.

Pour accorder ce droit, suivez les étapes suivantes :

1. Dans le Centre d'administration SharePoint, cliquez sur **profils utilisateur.**

2. Dans la section **Personnes,** cliquez sur **Gérer les autorisations utilisateur.**

3. Ajoutez les utilisateurs qui ont besoin d'autorisations pour créer leur site Mes sites. Par défaut, ce paramètre est définie sur Tout le monde **sauf les utilisateurs externes.**

4. Une fois que vous avez ajouté l'utilisateur, les utilisateurs ou le groupe, assurez-vous que l'utilisateur, les utilisateurs ou le groupe ajoutés est sélectionné, faites défiler la section **autorisations,** puis cochez la case en regard de Créer un site personnel (requis pour le stockage personnel, le **newsfeed** et le contenu suivi).

5. Cliquez **sur OK,** puis faites en cas d'accès de l'utilisateur à la page OneDrive pour créer le site.
