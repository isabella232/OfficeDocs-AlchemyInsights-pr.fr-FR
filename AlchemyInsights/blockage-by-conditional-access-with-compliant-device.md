---
title: Je suis bloqué par l’accès conditionnel avec un appareil compatible
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897675"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Je suis bloqué par l’accès conditionnel avec un appareil compatible

**Outils hautement recommandés**

- [Outil de résolution des problèmes d’alignement des appareils](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) : outil complet qui vous aide à résoudre les problèmes courants d’alignement des appareils.
- [Script de connectivité pour l'alignement des appareils de test](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : outil utilisé pour s’assurer qu’un appareil peut accéder aux points de terminaison d’alignement des appareils sous le compte système.
- [Script de nettoyage d’appareil Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : outil utilisé pour rechercher et gérer les appareils obsolètes dans votre environnement.

Voici quelques-unes des raisons pour lesquelles l’accès conditionnel peut échouer pour un appareil compatible ou pourquoi vos utilisateurs peuvent recevoir le message **Vous ne pouvez pas y accéder à partir d’ici** lors d’une demande de connexion à une ressource de l’organisation.

1. **L’appareil n’est pas dans l’état requis avec une gestion des appareils** :

Vérifier que l’appareil est inscrit auprès d’un fournisseur de gestion des appareils approuvé tel qu’Intune et qu’il est *marqué comme conforme*. Pour plus d’informations sur Intune, consultez ce [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Pour mieux comprendre la conformité des appareils et Intune, consultez [utiliser une stratégie de conformité pour définir des règles pour les appareils que vous gérez avec Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Si vous rencontrez des problèmes lors de l'inscription d'un appareil avec Intune, vous trouverez des détails de résolution des problèmes, consultez [Résolution des problèmes d'inscription des appareils dans Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Pour une prise en charge supplémentaire d’Intune, créez une demande de support. Pour ce faire, visitez la [page d’aide et de Support Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **L'appareil n'est pas joint au réseau de l'organisation**:

Pour accéder aux ressources de l'organisation, l'appareil doit être connecté au réseau de l'organisation, soit par une connexion directe, soit par un réseau privé virtuel (VPN), et également joint au réseau local ou à Azure Active Directory. Pour joindre un appareil professionnel au réseau de l’organisation, consultez [Joindre votre appareil de travail au réseau de votre organisation](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Pour enregistrer un appareil personnel/BYOD, consultez [Inscrire votre appareil personnel sur le réseau de votre organisation](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Pour vérifier si l’appareil a rejoint le réseau, vous pouvez suivre les étapes pour les appareils inscrits [ici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) ou les appareils de travail [ici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Pour déterminer si le problème est lié à la connectivité du réseau de l'organisation, suivez les instructions ci-dessous :

    1. Connectez-vous à Windows à l’aide de votre compte scolaire ou professionnel, par exemple  alain@contoso.com.
    2. Connectez-vous au réseau de votre organisation via un VPN ou DirectAccess.
    3. Une fois que vous êtes connecté, appuyez sur **touche logo Windows + L** pour verrouiller votre appareil.
    4. Déverrouillez votre appareil à l’aide de votre compte professionnel ou scolaire, puis essayez d’accéder de nouveau à l’application ou au service problématique.

Si vous voyez à nouveau le message d'erreur **Vous ne pouvez pas y accéder d'ici**, le problème est probablement ailleurs.

3. **Le système d’exploitation n’est pas pris en charge**:

Vérifiez que vous exécutez une version prise en charge du système d’exploitation, notamment :

- **Client Windows** : Windows 7 ou version ultérieure

- **Windows Server** : Windows Server 2008 R2 ou version ultérieure

- **macOS** : macOS X ou version ultérieure

- **Android et iOS** : dernière version des systèmes d’exploitation mobiles Android et iOS

4. **Le navigateur web n’est pas pris en charge** :

Consultez les navigateurs pris en charge ci-dessous. Pour la prise en charge de Chrome avec Windows 1703 ou version ultérieure, une extension Compte Windows 10 est requise. Pour Edge 85+, l’utilisateur doit être connecté pour transmettre correctement les informations de conformité de l’appareil. Pour plus d’informations, reportez-vous [ici](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10** : Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1** : Internet Explorer, Chrome
- **Windows 7** : Internet Explorer, Chrome
- **iOS** : Microsoft Edge, Navigateur géré par Intune, Safari
- **Android** : **Microsoft Edge** : Navigateur géré par Intune, Chrome
- **Windows Phone** : Microsoft Edge, Internet Explorer
- **Windows Server 2019** : Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016** : Internet Explorer
- **Windows Server 2012 R2** : Internet Explorer
- **Windows Server 2008 R2** : Internet Explorer
- **macOS**: Chrome, Safari

Recherchez plus d’informations sur le message **Vous ne pouvez pas y accéder d’ici** et les étapes de résolution des problèmes disponibles [ici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
