---
title: Termes manquants dans le magasin de termes SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053511"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activation du chiffrement BitLocker avec Intune

La stratégie de protection du point de terminaison Intune peut être utilisée pour configurer les paramètres de chiffrement Boitlocker pour les appareils Windows, comme décrit dans les paramètres suivants : Windows10 (et versions ultérieures) pour protéger les appareils à l’aide d’Intune

Vous devez savoir que de nombreux appareils plus récents exécutant Windows 10 prennent en charge le chiffrement BitLocker automatique, qui est déclenché sans l’application de la stratégie MDM. Cela peut avoir un impact sur l’application de la stratégie si des paramètres autres que ceux par défaut sont configurés. Pour plus d’informations, voir le Forum aux questions.


FAQ  Q : Quelles éditions de Windows prennent en charge le chiffrement des appareils à l’aide de la stratégie de protection du point de terminaison ?
 A : les paramètres de la stratégie de protection du point de terminaison Intune sont implémentés à l’aide du CSP BitLocker.Toutes les éditions et les versions de Windows ne prennent pas en charge le fournisseur de services cryptographiques BitLocker. 
      Pour le moment, les éditions Windows : entreprise ; Éducation, mobile, mobile Enterprise et professionnel (à partir de la build 1809 et versions ultérieures) sont pris en charge.




Q : si un appareil est déjà chiffré avec BitLocker à l’aide des paramètres de système d’exploitation par défaut pour la méthode de chiffrement et la force de chiffrement (XTS-AES-128), l’application d’une stratégie avec différents paramètres déclenchera automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?

R : Non. Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.

Remarque pour les appareils en cours d’enregistrement avec AutoPilot, le chiffrement automatique qui se produit pendant OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation.




Q si un périphérique est chiffré suite à l’application de la stratégie Intune sera-t-il déchiffré lors de la suppression de cette stratégie ?

A : la suppression de la stratégie liée au chiffrement n’entraîne pas le déchiffrement des lecteurs qui ont été configurés.




Q : pourquoi la stratégie de conformité Intune indique-t-elle que mon appareil ne dispose pas de « BitLocker Enabled », mais c’est ?

A : le paramètre « BitLocker Enabled » dans la stratégie de conformité Intune utilise le client Windows Device Health attestation (DHA). Ce client mesure uniquement l’état de l’appareil au moment du démarrage. Par conséquent, si un périphérique n’a pas été redémarré depuis le chiffrement BitLocker, le service client DHA ne signalera pas BitLocker comme étant actif.