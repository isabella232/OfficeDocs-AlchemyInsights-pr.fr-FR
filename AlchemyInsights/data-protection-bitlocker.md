---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778191"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activation du chiffrement Bitlocker avec Intune

La stratégie de protection des points de terminaison Intune peut être utilisée pour configurer les paramètres de chiffrement Bitlocker pour les appareils Windows. Pour plus d’informations, [voir les paramètres windows 10 (et ultérieurs) pour protéger les appareils à l’aide d’Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Outre la stratégie endpoint Protection, il existe également un rapport de chiffrement qui fournit une vue plus détaillée de l’état du chiffrement pour les appareils. Ce rapport est accessible à partir du portail MEM sous **Devices > Monitor,** puis sous **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Si vous constatez que Bitlocker ne parvient pas à être activé comme prévu ou que le profil utilisé pour activer Bitlocker est dans un état d’erreur, consultez le rapport de chiffrement pour mieux comprendre pourquoi le comportement se produit.

Pour plus d’informations sur l’interprétation du rapport, y compris les différentes valeurs d’état de chiffrement, voir Surveiller le chiffrement de [l’appareil avec Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Vous devez savoir que de nombreux appareils plus nouveaux exécutant Windows 10 peuvent prendre en charge le chiffrement Bitlocker automatique, qui est déclenché sans l’application de la stratégie de gestion des périphériques mobiles. Cela peut avoir un impact sur l’application de la stratégie si des paramètres autres que ceux par défaut sont configurés. Pour plus d’informations, voir la FAQ suivante.

Pour plus d’informations sur la résolution des problèmes de bitlocker, voir Résoudre les problèmes de [stratégies BitLocker dans Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**FAQ**

Q : Quelles éditions de Windows supportent le chiffrement d’appareil à l’aide de la stratégie endpoint Protection ?<br>
R : Les paramètres de la stratégie de protection des points de terminaison Intune sont implémentés à l’aide du [CSP Bitlocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Toutes les éditions ou builds de Windows ne sont pas en charge par le programme CSP Bitlocker. <br><br>

Q : Comment Bitlocker peut-il être activé sur des appareils sans nécessiter d’interaction de l’utilisateur final ?<br>
R : Tant que les conditions préalables nécessaires sont remplies, il est possible d’activer le « chiffrement silencieux » Bitlocker via Intune. Consultez les détails de la configuration requise pour l’appareil et des exemples de paramètres de stratégie pour activer le chiffrement en mode silencieux dans la documentation suivante : Activer silencieusement le chiffrement [Bitlocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

Q : Si un appareil est déjà chiffré avec Bitlocker à l’aide des paramètres par défaut du système d’exploitation pour la méthode de chiffrement et la force de chiffrement (XTS-AES-128), l’application d’une stratégie avec différents paramètres déclenche automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?<br>
R : Non. Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.<br><br>
**Remarque :** Pour les appareils inscrits avec Autopilot, le chiffrement automatique qui se produira pendant la phase OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation.
 
Q : Si un appareil est chiffré à la suite de l’application de la stratégie Intune, sera-t-il déchiffré lors de la suppression de cette stratégie ?<br>
R : La suppression de la stratégie de chiffrement n’entraîne PAS le déchiffrement des lecteurs qui ont été configurés.
 
Q : Pourquoi la stratégie de conformité Intune indique-t-elle que Bitlocker n’est pas activé sur mon appareil, même s’il l’est ?<br>
R : le paramètre « Bitlocker activé » dans la stratégie de conformité Intune utilise le client d’attestation d’état d’état de l’appareil Windows. Ce client mesure uniquement l’état de l’appareil au démarrage. Ainsi, si un appareil n’a pas été redémarrage depuis la fin du chiffrement Bitlocker, le service client DHA ne signale pas Bitlocker comme étant actif.
 
 