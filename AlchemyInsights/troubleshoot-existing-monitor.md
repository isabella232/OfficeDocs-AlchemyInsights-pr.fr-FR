---
title: Résolution des problèmes de moniteur existant
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690709"
---
# <a name="troubleshoot-an-existing-monitor"></a>Résoudre les problèmes d’un moniteur existant

Essayez ces solutions pour dépanner un moniteur. 

**Actualisez l’affichage de votre moniteur :**

Appuyez simultanément sur les touches suivantes : touche Windows + Ctrl + Maj + B. Cette opération permet d’actualiser la communication avec votre pilote graphique. Vos moniteurs clignotent momentanément et reviennent après quelques secondes.

**Dépanner le matériel de surveillance :**

1. Débranchez le câble reliant votre PC à votre moniteur, puis reconnectez-le.
2. Déconnectez les appareils non essentiels de votre PC (cartes ou stations d’accueil, par exemple).

**Si vous avez récemment installé une mise à jour sur votre PC, vous pouvez restaurer votre pilote d’affichage :**

1. Sélectionnez **Démarrer**, tapez **Gestionnaire de périphériques**, puis sélectionnez **Gestionnaire de périphériques** dans les résultats.
2. Développez la section **cartes graphiques** , cliquez avec le bouton droit sur votre carte vidéo, opérateurs and sélectionnez **Propriétés**.
3. Accédez à l’onglet **pilote** et sélectionnez **restaurer le pilote**. <br>
Remarque : si cette option n’est pas disponible ou est grisée, sélectionnez **non** parmi les options ci-dessous pour passer à l’étape suivante.
4. Vous devrez peut-être redémarrer votre PC pour que ces modifications prennent effet.

**Désinstallez et réinstallez votre pilote d’affichage :**

1. Sélectionnez **Démarrer**, tapez **Gestionnaire de périphériques**, puis sélectionnez **Gestionnaire de périphériques** dans les résultats.
2. Développez la section **cartes graphiques** , cliquez avec le bouton droit sur votre carte vidéo, opérateurs and sélectionnez **désinstaller le périphérique**. 
3. Activez la case à cocher en regard de **supprimer le pilote logiciel de ce périphérique** , puis sélectionnez **désinstaller**.<br>
Remarque : vous serez peut-être invité à redémarrer votre ordinateur à ce stade. Veillez à noter les autres instructions avant de redémarrer.
4. Ouvrez à nouveau le gestionnaire de périphériques.
5. Développez la section **cartes graphiques** , cliquez avec le bouton droit sur votre carte graphique, puis sélectionnez **mettre à jour le pilote**.
6. Sélectionnez **recherche automatique pour mettre à jour le pilote logiciel** et suivez les instructions d’installation.