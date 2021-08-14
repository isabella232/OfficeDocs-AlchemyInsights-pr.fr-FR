---
title: OneDrive Entreprise Les OneDrive web redirigent vers Delve
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
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922985"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirigé vers Delve après avoir cliqué sur OneDrive

Consultez notre guide [de dépannage détaillé.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Pour résoudre ce problème, l’administrateur doit accorder aux utilisateurs le droit de créer leur site Mes sites. Cela est dû au fait que OneDrive Entreprise page est créée sur Mes sites.

Pour accorder ce droit, suivez les étapes suivantes :

1. Dans le centre SharePoint’administration, cliquez sur **profils utilisateur.**

2. Dans la section **Personnes,** cliquez sur **Gérer les autorisations utilisateur.**

3. Ajoutez les utilisateurs qui ont besoin d’autorisations pour créer leur site Mes sites. Par défaut, ce paramètre est définie sur Tout le monde **sauf les utilisateurs externes.**

4. Une fois que vous avez ajouté l’utilisateur, les utilisateurs ou le groupe, assurez-vous que l’utilisateur, les utilisateurs ou le groupe ajoutés est sélectionné, faites défiler la section **autorisations,** puis cochez la case en regard de Créer un site personnel (requis pour le stockage personnel, le **newsfeed** et le contenu suivi).

5. Cliquez **sur OK,** puis faites en cas d’accès de l’utilisateur à OneDrive page pour créer le site.
