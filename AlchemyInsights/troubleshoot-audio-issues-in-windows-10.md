---
title: Résoudre les problèmes audio dans Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750305"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Résolution des problèmes audio dans Windows 10

**Exécuter l’utilitaire de résolution des problèmes audio**

1.  Ouvrez les [paramètres de résolution des problèmes](ms-settings:troubleshoot).

2.  Sélectionnez **lecture audio**  >  **Exécutez l’utilitaire de résolution des problèmes**.

**Définir le périphérique par défaut**

Si vous vous connectez à un périphérique audio à l’aide de l’USB ou de l’HDMI, vous devrez peut-être définir ce périphérique par défaut :

1. Ouvrez **Démarrer**le  >  **son**, puis sélectionnez **son** ou **Modifiez sons système** dans la liste des résultats.

2.  Sous l’onglet **lecture** , sélectionnez un appareil, sélectionnez **définir la valeur par défaut**, puis **OK**.

**Vérifier les câbles, le volume, les haut-parleurs et le casque**

1. Vérifiez que les câbles de votre haut-parleur et de votre casque sont connectés et assurez-vous qu’ils sont connectés à la bonne prise.

2. Vérifiez les niveaux de puissance et de volume et essayez de relancer tous les contrôles de volume.

3. Certains haut-parleurs et applications ont leurs propres contrôles de volume ; vous devrez peut-être les vérifier tout pour vous assurer qu’ils sont aux niveaux corrects.

4. Essayez de vous connecter à l’aide d’un autre port USB.

**Remarque**: n’oubliez pas que vos haut-parleurs ne fonctionnent pas lorsque le casque est branché.

**Vérifier le gestionnaire de périphériques**

Pour vous assurer que les pilotes sont à jour :

1. Sélectionnez **Démarrer**, tapez **Gestionnaire de périphériques**, puis sélectionnez **Gestionnaire de périphériques** dans la liste des résultats.

2. Sous **Contrôleurs audio, vidéo et jeu**, sélectionnez votre carte audio, ouvrez-la, sélectionnez l’onglet **pilote** , puis sélectionnez **mettre à jour le pilote**.

**Remarque**: si Windows ne trouve pas de nouveau pilote, recherchez-en un sur le site Web du fabricant de l’appareil et suivez les instructions.

**Réinstaller le pilote**

Si vous ne pouvez pas effectuer une mise à jour via le gestionnaire de périphériques ou si vous recherchez un nouveau pilote sur le site Web du fabricant, procédez comme suit :

1. Dans le gestionnaire de périphériques, cliquez avec le bouton droit (ou appuyez longuement) sur le pilote audio, puis sélectionnez **désinstaller**. Redémarrez votre appareil et Windows tentera de réinstaller le pilote.

2. Si la réinstallation du pilote ne fonctionne pas, essayez d’utiliser le pilote audio générique fourni avec Windows. Dans le gestionnaire de périphériques, cliquez avec le bouton droit de la touche (ou appuyez longuement) sur votre pilote audio > **mettre à jour le logiciel**  >  **de pilote pour rechercher le pilote logiciel**, sélectionnez  >  **l’une des pilotes de périphériques sur mon ordinateur**, sélectionnez **périphérique audio haute définition**, sélectionnez **suivant**, puis suivez les instructions pour l’installer.
