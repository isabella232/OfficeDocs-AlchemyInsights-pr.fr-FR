---
title: Termes manquants dans SharePoint magasin de termes en ligne
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106424"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activation du chiffrement Bitlocker avec Intune

La stratégie de Endpoint Protection Intune peut être utilisée pour configurer les paramètres de chiffrement Delocker pour les appareils Windows comme décrit dans : Paramètres Windows 10 (et ultérieur) pour protéger les appareils à l’aide d’Intune

Vous devez savoir que de nombreux appareils plus nouveaux exécutant Windows 10 le chiffrement bitlocker automatique qui est déclenché sans l’application de la stratégie de gestion des périphériques mobiles. Cela peut avoir un impact sur l’application de la stratégie si des paramètres non par défaut sont configurés. Pour plus d’informations, voir FAQ.


FAQ Q : Quelles éditions de Windows prise en charge du chiffrement d’appareil à l’aide de la stratégie Endpoint Protection de sécurité ?
R : Les paramètres de la stratégie de Endpoint Protection Intune sont implémentés à l’aide du CSP Bitlocker.  Toutes les éditions ni les builds de Windows le programme CSP Bitlocker. Pour le moment, Windows Éditions : Enterprise; Éducation, Mobile, Mobile Enterprise et Professional (à partir de la build 1809) sont pris en charge.




Q : Si un appareil est déjà chiffré avec Bitlocker à l’aide des paramètres par défaut du système d’exploitation pour la méthode de chiffrement et la force de chiffrement (XTS-AES-128), une stratégie avec différents paramètres déclenche automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?

R : Non. Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.

Remarque Pour les appareils inscrits avec Autopilot, le chiffrement automatique qui se produira pendant la phase OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation




Q Si un appareil est chiffré à la suite de l’application de la stratégie Intune, sera-t-il déchiffré lors de la suppression de cette stratégie ?

R : La suppression de la stratégie liée au chiffrement n’entraîne PAS le déchiffrement des lecteurs qui ont été configurés.




Q : Pourquoi la stratégie de conformité intune indique-t-elle que mon appareil n’a pas « Bitlocker activé », mais qu’il l’est ?

R : le paramètre « Bitlocker activé » dans la stratégie de conformité Intune utilise le client d’attestation d’Windows(DHA). Ce client mesure uniquement l’état de l’appareil au démarrage. Ainsi, si un appareil n’a pas été redémarrage depuis la fin du chiffrement bitlocker, le service client DHA ne signale pas bitlocker comme étant actif.