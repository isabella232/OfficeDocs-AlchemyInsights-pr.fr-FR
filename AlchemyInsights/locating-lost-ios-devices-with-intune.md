---
title: Localisation de pertes d’appareils iOS avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675157"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Localisation de pertes d’appareils iOS avec Intune

L’activation du mode perdu sur un appareil iOS permet à un administrateur d’avoir un message et un numéro de téléphone de contact affichés sur l’écran de verrouillage.

Une fois le mode perdu activé, l’administrateur peut utiliser l’action localiser l’appareil pour identifier l’emplacement physique de l’appareil.

L’action localiser l’appareil dans Intune fonctionne avec les appareils iOS pour afficher l’emplacement d’un appareil spécifique sur une carte.

L’utilisation de cette action nécessite que l’appareil iOS soit en :

- Mode supervisé
- Mode Perdu

Pour plus d’informations, consultez [Activer le mode perdu sur les appareils iOS/iPad avec Intune](https://docs.microsoft.com/intune/device-lost-mode) et [Localiser les appareils iOS/iPad d’iOS perdus ou volés avec Intune](https://docs.microsoft.com/intune/device-locate).

**FAQ**

Q : j'ai lancé une action à distance pour supprimer les données de l'entreprise d'un appareil, et l'état d'attente est maintenant bloqué.

R : pour qu'une action à distance soit menée à bien, l'appareil ciblé doit être en ligne et sain. Dans les situations suivantes, l’action distante reste dans un état d’attente pendant 30 jours, ou jusqu’à ce que l’appareil accuse la commande suivante :

- Lorsque l’appareil ne possède pas de connectivité
- Lorsque l’appareil perd son état de gestion avec Intune

Si vous pensez qu'un appareil n'est plus enregistré, et qu'il ne peut pas supprime les données de l'entreprise, sélectionnez Supprimer. La suppression supprime l'enregistrement de l'appareil afin qu'il n'apparaisse plus dans la liste des appareils d'Intune. Si l’appareil redevient actif, l’utilisateur doit le ré-inscrire.

Q : pourquoi certaines actions à distance ne sont-elles pas disponibles pour mon utilisation ?

R : toutes les plateformes ne prennent pas en charge toutes les actions de périphériques distants. Les actions distantes suivantes sont spécifiques aux plateformes, de sorte qu’elles sont disponibles uniquement pour les plateformes indiquées.

- Contourner le verrou d’activation (iOS uniquement)
- Nouveau démarrage (Windows uniquement)
- Mode perdu (iOS uniquement)
- Localiser l’appareil (iOS uniquement)
- Redémarrer (Windows uniquement)

Pour plus d’informations sur chaque action, consultez [Actions d’appareil disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).