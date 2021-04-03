---
title: Clés de récupération Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505066"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Accès aux clés de récupération Bitlocker

Lors de la configuration de la stratégie intune Endpoint Protection des paramètres Bitlocker, il est possible de définir si les informations de récupération Bitlocker doivent être stockées dans Azure Active Directory.

Si ce paramètre est configuré, les données de récupération stockées doivent être visibles par un administrateur Intune dans le cadre des données d’enregistrement d’appareil dans le panneau Appareils Intune de deux manières :

Appareils - Appareils Azure AD -> « Appareil » OU Appareils -> Tous les appareils -> « Appareil » -> clés de récupération

Sinon, s’il existe un accès administratif à l’appareil lui-même, vous pouvez voir la clé de récupération (Mot de passe) en exécutant la commande suivante à partir d’une invite de commandes avec élévation de élévation de niveaux :

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Si l’appareil a été chiffré avant l’inscription dans Intune, la clé de récupération a peut-être été associée au « compte Microsoft » (MSA) utilisé pour se connecter à l’appareil pendant le processus OOBE. Si c’est le cas, l’accès à ce MSA et sa signature doivent afficher les appareils pour lesquels les clés de récupération  https://onedrive.live.com/recoverykey ont été stockées.
 
Si l’appareil a été chiffré à la suite d’une configuration par le biais d’une stratégie de groupe basée sur un domaine, les informations de récupération peuvent être stockées dans Active Directory local.

Si vous avez configuré la stratégie de protection des points de terminaison pour stocker la clé de récupération dans Azure Active Directory, mais que la clé d’un appareil spécifique n’a pas été téléchargée, vous pouvez déclencher le chargement en faisant pivoter la clé de récupération de cet appareil à partir de la console MEM. Pour plus d’informations, voir [Faire pivoter les clés de récupération BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

