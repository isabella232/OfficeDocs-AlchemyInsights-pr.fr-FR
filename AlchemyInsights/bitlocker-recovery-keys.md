---
title: Clés de récupération BitLocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685884"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Accès aux clés de récupération BitLocker

Lors de la configuration des paramètres BitLocker stratégie de protection du point de terminaison Intune, il est possible de définir si les informations de récupération BitLocker doivent être stockées dans Azure Active Directory.

Si ce paramètre est configuré, les données de récupération stockées doivent être visibles par un administrateur Intune dans le cadre des données d’enregistrement du périphérique dans le panneau des appareils Intune de deux façons :

Périphériques-périphériques Azure AD-> « périphérique » ou périphériques-> tous les périphériques-> « périphérique »-> clés de récupération

Par ailleurs, s’il existe un accès administratif au périphérique lui-même, la clé de récupération (mot de passe) est visible en exécutant la commande suivante à partir d’une invite de commandes avec élévation de privilèges :

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
Si le périphérique a été chiffré avant d’être inscrit dans Intune, la clé de récupération a peut-être été associée au « compte Microsoft » (MSA) utilisé pour se connecter à l’appareil pendant le processus OOBE. Si c’est le cas, l’accès  https://onedrive.live.com/recoverykey et la connexion à l’aide de ce MSA doivent afficher les périphériques pour lesquels des clés de récupération ont été stockées.
 
Si l’appareil a été chiffré à la suite d’une configuration via une stratégie de groupe basée sur un domaine, les informations de récupération peuvent être stockées dans l’annuaire Active Directory local.
 

