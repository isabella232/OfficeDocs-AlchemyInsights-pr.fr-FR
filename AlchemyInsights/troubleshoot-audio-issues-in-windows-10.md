---
title: Résoudre les problèmes audio dans Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039424"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Résolution des problèmes audio dans Windows 10

**Exécuter l’résolution des problèmes audio**

1.  Ouvrez les [paramètres de résolution des problèmes.](ms-settings:troubleshoot)

2.  Select **Playing Audio** Run the  >  **troubleshooter**.

**Définir l’appareil par défaut**

Si vous vous connectez à un périphérique audio à l’aide d’une clé USB ou HDMI, vous devrez peut-être définir cet appareil comme périphérique par défaut :

1. Ouvrez **le**  >  **son** de démarrage, puis sélectionnez **Son** ou Modifier les **sons système** dans la liste des résultats.

2.  Sous **l’onglet Lecture,** sélectionnez un appareil, **sélectionnez** Définir par défaut, puis **OK**.

**Vérifier les câbles, le volume, les haut-parleurs et le casque**

1. Vérifiez la connexion de votre haut-parleur et de votre casque pour les câbles souples et assurez-vous qu’ils sont connectés à la prise correcte.

2. Vérifiez vos niveaux de puissance et de volume et essayez d’allumer tous les contrôles de volume.

3. Certains haut-parleurs et applications ont leurs propres contrôles de volume . Vous de devez peut-être tous les vérifier pour vous assurer qu’ils se retrouvent aux bons niveaux.

4. Essayez de vous connecter à l’aide d’un autre port USB.

**Remarque**: n’oubliez pas que vos haut-parleurs peuvent ne pas fonctionner lorsque le casque est branché.

**Vérifier le Gestionnaire de périphériques**

Pour vous assurer que les pilotes sont à jour :

1. Sélectionnez **Démarrer,** **tapez Gestionnaire de** périphériques, puis sélectionnez **Gestionnaire de** périphériques dans la liste des résultats.

2. Sous **son, vidéo et contrôleurs** de jeu, sélectionnez  votre carte son, ouvrez-la, sélectionnez l’onglet Pilote, puis sélectionnez Mettre à **jour le pilote.**

**Remarque**: si Windows ne trouve pas de nouveau pilote, recherchez-en un sur le site web du fabricant de l’appareil et suivez leurs instructions.

**Réinstaller le pilote**

Si vous ne pouvez pas mettre à jour via le Gestionnaire de périphériques ou trouver un nouveau pilote sur le site web du fabricant, effectuez les étapes suivantes :

1. Dans le Gestionnaire de périphériques, cliquez avec le bouton droit (ou maintenez la souris sur le pilote audio), puis sélectionnez **Désinstaller.** Redémarrez votre appareil et Windows tentez de réinstaller le pilote.

2. Si la réinstallation du pilote ne fonctionne pas, essayez d’utiliser le pilote audio générique qui est Windows. Dans le Gestionnaire de périphériques, cliquez avec le bouton droit (ou appuyez longuement) sur votre pilote audio > Mettre à jour le logiciel de pilote Parcourir mon ordinateur pour le logiciel de pilote. Laissez-moi choisir dans une liste de pilotes de périphérique sur mon ordinateur, sélectionnez Périphérique audio haute définition, sélectionnez Suivant et suivez les  >    >  instructions  pour l’installer.
