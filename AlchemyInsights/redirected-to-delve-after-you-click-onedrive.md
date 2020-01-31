---
title: Onedrive entreprise Web OneDrive redirige vers Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571201"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirigé vers Delve après avoir cliqué sur OneDrive

Consultez notre [Guide de dépannage](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)détaillé.

Pour résoudre ce problème, l’administrateur Office 365 doit accorder aux utilisateurs le droit de créer leur site mes sites. Cela est dû au fait que la page OneDrive entreprise est créée sur les sites mon site.

Pour accorder ce droit, procédez comme suit :

1. Dans le centre d’administration SharePoint, cliquez sur **profils utilisateur**.

2. Dans la section **personnes** , cliquez sur **gérer les autorisations des utilisateurs**.

3. Ajoutez des utilisateurs qui requièrent des autorisations pour créer leur site mes sites. Par défaut, ce paramètre est défini sur **tout le monde sauf les utilisateurs externes**.

4. Une fois que vous avez ajouté l’utilisateur, les utilisateurs ou le groupe, vérifiez que l’utilisateur, les utilisateurs ou le groupe ajouté est sélectionné, faites défiler jusqu’à la section **autorisations** , puis activez la case à cocher en regard de **créer un site personnel (requis pour le stockage personnel, le flux d’actualités et le contenu suivi)**.

5. Cliquez sur **OK**, puis demandez à l’utilisateur d’accéder à la page OneDrive pour créer le site.
