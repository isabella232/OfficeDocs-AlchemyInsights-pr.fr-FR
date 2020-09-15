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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="5f1a3-102">Accès aux clés de récupération BitLocker</span><span class="sxs-lookup"><span data-stu-id="5f1a3-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="5f1a3-103">Lors de la configuration des paramètres BitLocker stratégie de protection du point de terminaison Intune, il est possible de définir si les informations de récupération BitLocker doivent être stockées dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f1a3-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="5f1a3-104">Si ce paramètre est configuré, les données de récupération stockées doivent être visibles par un administrateur Intune dans le cadre des données d’enregistrement du périphérique dans le panneau des appareils Intune de deux façons :</span><span class="sxs-lookup"><span data-stu-id="5f1a3-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="5f1a3-105">Périphériques-périphériques Azure AD-> « périphérique » ou périphériques-> tous les périphériques-> « périphérique »-> clés de récupération</span><span class="sxs-lookup"><span data-stu-id="5f1a3-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="5f1a3-106">Par ailleurs, s’il existe un accès administratif au périphérique lui-même, la clé de récupération (mot de passe) est visible en exécutant la commande suivante à partir d’une invite de commandes avec élévation de privilèges :</span><span class="sxs-lookup"><span data-stu-id="5f1a3-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="5f1a3-107">Si le périphérique a été chiffré avant d’être inscrit dans Intune, la clé de récupération a peut-être été associée au « compte Microsoft » (MSA) utilisé pour se connecter à l’appareil pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="5f1a3-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="5f1a3-108">Si c’est le cas, l’accès  https://onedrive.live.com/recoverykey et la connexion à l’aide de ce MSA doivent afficher les périphériques pour lesquels des clés de récupération ont été stockées.</span><span class="sxs-lookup"><span data-stu-id="5f1a3-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="5f1a3-109">Si l’appareil a été chiffré à la suite d’une configuration via une stratégie de groupe basée sur un domaine, les informations de récupération peuvent être stockées dans l’annuaire Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="5f1a3-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

