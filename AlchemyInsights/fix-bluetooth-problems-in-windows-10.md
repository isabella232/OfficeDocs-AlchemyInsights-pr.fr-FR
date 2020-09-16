---
title: Corriger les problèmes Bluetooth dans Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730157"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Corriger les problèmes Bluetooth dans Windows 10

Si l’icône Bluetooth est manquante ou si Bluetooth ne peut pas être activé ou désactivé, vous pouvez exécuter l’utilitaire de résolution des problèmes Bluetooth. [Ouvrez les paramètres de résolution des problèmes](ms-settings:troubleshoot), cliquez sur **Bluetooth** sous **Rechercher et résoudre d’autres problèmes**, cliquez sur **exécuter l’utilitaire de résolution**des problèmes.

Si vous ne voyez pas l’icône Bluetooth, c’est que Bluetooth apparaît dans le gestionnaire de périphériques :

1. Dans le gestionnaire de périphériques, cliquez sur **Bluetooth**. Appuyez longuement (ou cliquez avec le bouton droit) sur le nom de la carte Bluetooth, puis cliquez sur **désinstaller l’appareil**.

2. Éteignez votre appareil Windows, patientez quelques secondes, puis rallumez-le. Windows essaiera de réinstaller le pilote.

Si vous avez récemment installé les mises à jour de Windows 10 ou mis à niveau vers Windows 10, vous souhaiterez peut-être vérifier les mises à jour de pilotes :

1. Dans le gestionnaire de périphériques, cliquez sur **Bluetooth**, puis sur le nom de la carte Bluetooth (qui peut inclure le mot « radio »).

2. Appuyez longuement (ou cliquez avec le bouton droit) sur la carte Bluetooth, puis cliquez sur **mettre à jour**la  >  **recherche de pilote automatiquement pour le logiciel de pilote mis à jour**. Suivez les étapes, puis cliquez sur **Fermer**.

      - Si Windows ne trouve pas de nouveau pilote Bluetooth, visitez le site Web du fabricant de PC et téléchargez le pilote Bluetooth le plus récent à partir de là.

    - Une fois le téléchargement effectué, cliquez sur **mettre à jour le pilote**parcourir le lecteur  >  **mon ordinateur pour le pilote logiciel**  >  **recherchez** l’emplacement où sont stockés les fichiers du pilote > **OK**  >  **Next**, puis suivez les étapes d’installation.

3. Après avoir installé le pilote mis à jour, redémarrez l’ordinateur, puis vérifiez si cela résout le problème de connexion.

Pour plus d’informations sur la résolution des problèmes liés à Bluetooth, reportez-vous à l’article complet relatif à la [résolution des problèmes Bluetooth dans Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
