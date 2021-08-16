---
title: Contourner le verrou d’activation sur les appareils iOS supervisés avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: de52ba77d3155d957372c31d465881fc7e8fcbbe657dfa35dedfee2be52e5a52
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046498"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Contourner le verrou d’activation sur les appareils iOS supervisés avec Intune

La possibilité de contourner le verrou d’activation sur les appareils iOS simplifie la récupération du scénario dans lequel un utilisateur active le verrouillage d’activation sur un appareil d’entreprise, puis quitte l’entreprise.

Les conditions préalables au contournement d'un verrou d'activation sont les suivantes :

- Un appareil est « supervisé ».
- Le verrou d’activation est correctement activé à l’aide de la stratégie de restriction des appareils iOS dans Intune.

En outre, lorsque vous contournez un verrou d'activation, vous devez :

- Posséder physiquement l'appareil à nettoyer.
- Copier le code avant de lancer la réinitialisation.

**Remarque :** le code de réinitialisation ne respecte pas la casse. par conséquent, les caractères « - » ne sont pas obligatoires.

Pour plus d’informations, consultez [Contourner le verrou d’activation sur les appareils iOS supervisés avec Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**FAQ**

Q : **j'ai lancé une action à distance pour supprimer les données de l'entreprise d'un appareil, et l'état d'attente est maintenant bloqué.**

R : pour qu'une action à distance soit menée à bien, l'appareil ciblé doit être en ligne et sain. Dans les situations suivantes, l’action distante reste dans un état d’attente pendant 30 jours, ou jusqu’à ce que l’appareil accuse la commande lorsque l’appareil :

- Ne possède pas de connectivité.
- Perd son statut de gestion avec Intune.

Si vous pensez qu'un appareil n'est plus enregistré, et qu'il ne supprime pas les données de l'entreprise, sélectionnez Supprimer. La suppression supprime l'enregistrement de l'appareil afin qu'il n'apparaisse plus dans la liste des appareils d'Intune. Pour que l'appareil redevienne actif, son utilisateur doit le réinscrire.

Q : **pourquoi certaines actions à distance ne sont-elles pas disponibles pour mon utilisation ?**

R : toutes les plateformes ne prennent pas en charge toutes les actions de périphériques distants. Les actions distantes suivantes sont spécifiques aux plateformes.

- Contourner le verrou d’activation (iOS uniquement)
- Nouveau démarrage (Windows uniquement)
- Mode perdu (iOS uniquement)
- Localiser l’appareil (iOS uniquement)
- Redémarrer (Windows uniquement)

Pour plus d’informations sur chaque action, consultez [Actions d’appareil disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).