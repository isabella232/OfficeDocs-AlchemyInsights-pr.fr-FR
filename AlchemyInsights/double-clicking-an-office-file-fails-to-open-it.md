---
title: Le double-clic sur un fichier Office ne parvient pas à l'ouvrir
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814803"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Le double-clic sur un fichier Office ne parvient pas à l'ouvrir

Après avoir double-cliqué sur un fichier Office, le programme peut s'ouvrir, mais le fichier proprement dit ne s'ouvre pas. Sinon, vous pouvez obtenir l'erreur : « Un problème s'est produite lors de l'envoi de la commande au programme. » Il existe de nombreuses causes à cela, mais les deux solutions les plus courantes sont :

- Dans Excel, assurez-vous que l'option DDE est désactivée. L'option est disponible en créant un classez, puis en choisissant > Options > **Avancé**. Dans la section **Général,** décochez la section Ignorer les autres applications qui utilisent **Dynamic Data Exchange (DDE).**

- Exécutez une réparation en ligne pour restaurer les paramètres par défaut. Cliquez sur le bouton Démarrer de Windows et recherchez « Panneau de contrôle ». Ouvrez **le Panneau de** contrôle et allez à Programmes > programmes et **fonctionnalités.** Cliquez ensuite avec le **bouton droit Microsoft Office [Version]** et choisissez **Modifier > Réparation en ligne.**

Si aucune de ces solutions ne fonctionne, une liste plus complète de solutions est trouvée dans l'article de support, le double-clic sur un fichier Office ne [parvient pas à l'ouvrir.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
