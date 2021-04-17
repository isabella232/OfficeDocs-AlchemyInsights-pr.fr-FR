---
title: Clés de récupération Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820284"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="7f2e1-102">Accès aux clés de récupération Bitlocker</span><span class="sxs-lookup"><span data-stu-id="7f2e1-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="7f2e1-103">Lors de la configuration de la stratégie intune Endpoint Protection des paramètres Bitlocker, il est possible de définir si les informations de récupération Bitlocker doivent être stockées dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7f2e1-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="7f2e1-104">Si ce paramètre est configuré, les données de récupération stockées doivent être visibles par un administrateur Intune dans le cadre des données d'enregistrement d'appareil dans le panneau Appareils Intune de deux manières :</span><span class="sxs-lookup"><span data-stu-id="7f2e1-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="7f2e1-105">Appareils - Appareils Azure AD -> « Appareil » OU Appareils -> Tous les appareils -> « Appareil » -> clés de récupération</span><span class="sxs-lookup"><span data-stu-id="7f2e1-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="7f2e1-106">Sinon, s'il existe un accès administratif à l'appareil lui-même, vous pouvez voir la clé de récupération (Mot de passe) en exécutant la commande suivante à partir d'une invite de commandes avec élévation de élévation de niveaux :</span><span class="sxs-lookup"><span data-stu-id="7f2e1-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="7f2e1-107">Si l'appareil a été chiffré avant l'inscription dans Intune, la clé de récupération a peut-être été associée au « compte Microsoft » (MSA) utilisé pour se connecter à l'appareil pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="7f2e1-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="7f2e1-108">Si c'est le cas, l'accès à ce MSA et sa signature doivent afficher les appareils pour lesquels les clés de récupération  https://onedrive.live.com/recoverykey ont été stockées.</span><span class="sxs-lookup"><span data-stu-id="7f2e1-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="7f2e1-109">Si l'appareil a été chiffré à la suite d'une configuration par le biais d'une stratégie de groupe basée sur un domaine, les informations de récupération peuvent être stockées dans Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="7f2e1-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="7f2e1-110">Si vous avez configuré la stratégie de protection des points de terminaison pour stocker la clé de récupération dans Azure Active Directory, mais que la clé d'un appareil spécifique n'a pas été téléchargée, vous pouvez déclencher le chargement en faisant pivoter la clé de récupération de cet appareil à partir de la console MEM.</span><span class="sxs-lookup"><span data-stu-id="7f2e1-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="7f2e1-111">Pour plus d'informations, voir [Faire pivoter les clés de récupération BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="7f2e1-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

