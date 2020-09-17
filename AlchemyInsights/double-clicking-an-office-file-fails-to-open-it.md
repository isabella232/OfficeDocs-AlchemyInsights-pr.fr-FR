---
title: Un double-clic sur un fichier Office échoue pour l’ouvrir
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812077"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Un double-clic sur un fichier Office échoue pour l’ouvrir

Après avoir double-cliqué sur un fichier Office, vous pouvez voir le programme ouvert, mais le fichier lui-même ne s’ouvre pas. Ou vous pouvez obtenir l’erreur suivante : « un problème est survenu lors de l’envoi de la commande au programme. » Il existe de nombreuses causes pour cela, mais les deux solutions les plus courantes sont les suivantes :

- À partir d’Excel, vérifiez que l’option DDE n’est pas cochée. L’option peut être trouvée en créant un nouveau classeur, puis en choisissant **options de > de fichiers > avancé**. Dans la section **général** , désactivez la case à cocher **Ignorer les autres applications qui utilisent l’échange dynamique de données (DDE)**.

- Exécutez une réparation en ligne pour restaurer les paramètres par défaut. Cliquez sur le bouton Démarrer de Windows et recherchez « panneau de configuration ». Ouvrez le **panneau de configuration**et accédez à **programmes > programmes et fonctionnalités**. Cliquez ensuite avec le bouton droit sur **Microsoft Office [version]** et choisissez **modifier > réparation en ligne**.

Si aucune de ces solutions ne fonctionne, une liste plus complète de solutions est disponible dans l’article de support technique, un [double-clic sur un fichier Office ne parvient pas à l’ouvrir](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
