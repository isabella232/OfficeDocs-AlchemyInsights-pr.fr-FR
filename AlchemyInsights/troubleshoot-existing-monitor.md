---
title: Résolution des problèmes d’un moniteur existant
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
- "3454"
- "9001450"
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981075"
---
# <a name="troubleshoot-an-existing-monitor"></a>Résoudre les problèmes d’un moniteur existant

Essayez ces solutions pour résoudre les problèmes d’un moniteur. 

**Actualisez l’affichage de votre moniteur :**

Appuyez sur les touches suivantes en même temps : Windows touche + Ctrl + Décalage + B. Cela permettra d’actualiser la communication avec votre pilote graphique. Vos moniteurs clignotent momentanément et reviennent après quelques secondes.

**Résoudre les problèmes de matériel du moniteur :**

1. Débranchez le câble qui connecte votre PC à votre moniteur, puis branchez-le à nouveau.
2. Déconnectez les appareils non essentiels de votre PC (par exemple, les cartes ou les docks).

**Si vous avez récemment installé une mise à jour sur votre PC, vous pouvez revenir en arrière de votre pilote d’affichage :**

1. Sélectionnez **Démarrer,** **tapez gestionnaire de périphériques** et sélectionnez **Gestionnaire de périphériques** dans les résultats.
2. Développez la section **Cartes d’affichage,** cliquez avec le bouton droit sur votre carte d’affichage et sélectionnez **Propriétés.**
3. Accédez à **l’onglet Pilote** et **sélectionnez Revenir en arrière.** <br>
Remarque : si cette option n’est pas  disponible ou est grisée, sélectionnez Non dans les options ci-dessous pour passer à l’étape suivante.
4. Vous devrez peut-être redémarrer votre PC avant que ces modifications prennent effet.

**Désinstallez et réinstallez votre pilote d’affichage :**

1. Sélectionnez **Démarrer,** **tapez gestionnaire de périphériques** et sélectionnez **Gestionnaire de périphériques** dans les résultats.
2. Développez la section **Cartes d’affichage,** cliquez avec le bouton droit sur votre carte d’affichage, puis **sélectionnez Désinstaller l’appareil.** 
3. Sélectionnez la case à côté **de Supprimer le logiciel de pilote pour cet appareil,** puis **sélectionnez Désinstaller.**<br>
Remarque : vous pouvez être invité à redémarrer votre ordinateur à ce stade. Veillez à noter les instructions restantes avant de redémarrer.
4. Ouvrez de nouveau le Gestionnaire de périphériques.
5. Développez la section **Cartes d’affichage,** cliquez avec le bouton droit sur votre carte d’affichage, puis sélectionnez Mettre à **jour le pilote.**
6. Sélectionnez **Rechercher automatiquement pour le logiciel du pilote de mise à** jour et suivez les instructions d’installation.