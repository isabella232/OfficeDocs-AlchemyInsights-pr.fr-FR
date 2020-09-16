---
title: DataProtection-BitLocker
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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731237"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activation du chiffrement BitLocker avec Intune

 La stratégie de protection du point de terminaison Intune peut être utilisée pour configurer les paramètres de chiffrement BitLocker pour les appareils Windows. Pour plus d’informations, voir [Paramètres Windows 10 (et versions ultérieures) pour protéger les appareils à l’aide d’Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Vous devez savoir que de nombreux appareils plus récents exécutant Windows 10 prennent en charge le chiffrement BitLocker automatique, qui est déclenché sans l’application de la stratégie MDM. Cela peut avoir un impact sur l’application de la stratégie si des paramètres autres que ceux par défaut sont configurés. Pour plus d’informations, consultez le Forum aux questions suivant.
 
Pour plus d’informations sur la résolution des problèmes liés à BitLocker, voir [Troubleshoot BitLocker Policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

 Q : Quelles éditions de Windows prennent en charge le chiffrement des appareils à l’aide de la stratégie de protection du point de terminaison ?<br>
 A : les paramètres de la stratégie de protection du point de terminaison Intune sont implémentés à l’aide du [CSP BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Toutes les éditions ou les versions de Windows ne prennent pas en charge le fournisseur de services cryptographiques BitLocker. <br><br>
      Pour l’instant, les éditions suivantes de Windows sont prises en charge : entreprise, éducation, mobile, mobile Enterprise et professionnel (Build 1809 et versions ultérieures).
 
Q : si un appareil est déjà chiffré avec BitLocker à l’aide des paramètres de système d’exploitation par défaut pour la méthode de chiffrement et le niveau de chiffrement (XTS-AES-128), l’application d’une stratégie avec différents paramètres déclenchera automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?<br>
R : Non. Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.<br><br>
**Remarque :** Pour les appareils en cours d’enregistrement avec AutoPilot, le chiffrement automatique qui se produit pendant OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation.
 
Q : si un périphérique est chiffré à la suite de l’application de la stratégie Intune, sera-t-il déchiffré lors de la suppression de cette stratégie ?<br>
A : la suppression de la stratégie liée au chiffrement n’entraîne pas le déchiffrement des lecteurs qui ont été configurés.
 
Q : pourquoi la stratégie de conformité Intune indique-t-elle que BitLocker n’est pas activé sur mon appareil, même s’il s’agit de ?<br>
A : le paramètre « BitLocker Enabled » dans la stratégie de conformité Intune utilise le client Windows Device Health attestation (DHA). Ce client mesure uniquement l’état de l’appareil au moment du démarrage. Par conséquent, si un périphérique n’a pas été redémarré depuis le chiffrement BitLocker terminé, le service client DHA ne signalera pas BitLocker comme étant actif.
 
 