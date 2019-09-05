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
ms.openlocfilehash: 8ba296c6986c767939ef51076551f95719d11aa2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752246"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirigé vers Delve après avoir cliqué sur OneDrive

Pour résoudre ce problème, l’administrateur Office 365 doit accorder aux utilisateurs le droit de créer leur site mes sites. Cela est dû au fait que la page OneDrive entreprise est créée sur les sites mon site.

Pour accorder ce droit, procédez comme suit :

1. Dans le centre d’administration SharePoint, cliquez sur **profils utilisateur**.

2. Dans la section **personnes** , cliquez sur **gérer les autorisations des utilisateurs**.

3. Ajoutez des utilisateurs qui requièrent des autorisations pour créer leur site mes sites. Par défaut, ce paramètre est défini sur **tout le monde sauf les utilisateurs externes**.

4. Une fois que vous avez ajouté l’utilisateur, les utilisateurs ou le groupe, vérifiez que l’utilisateur, les utilisateurs ou le groupe ajouté est sélectionné, faites défiler jusqu’à la section **autorisations** , puis activez la case à cocher en regard de **créer un site personnel (requis pour le stockage personnel, les flux d’actualités et suivi du contenu)**.

5. Cliquez sur **OK**, puis demandez à l’utilisateur d’accéder à la page OneDrive pour créer le site.
