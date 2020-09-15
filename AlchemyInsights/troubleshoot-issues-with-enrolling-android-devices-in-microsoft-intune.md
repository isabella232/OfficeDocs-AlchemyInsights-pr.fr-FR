---
title: Résoudre les problèmes liés à l’enregistrement d’appareils Android dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689952"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Résoudre les problèmes liés à l’enregistrement d’appareils Android dans Microsoft Intune

Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant.
  
Voici quelques étapes de résolution et de problèmes courants :
  
 **Erreur de périphérique non chiffré dans le portail d’entreprise :** Les versions plus récentes d’Android, en particulier à partir de la version 7.0, nécessitent un code secret de démarrage pour s’assurer que votre appareil est entièrement chiffré. Les solutions courantes sont l’activation d’un code confidentiel de démarrage ou le chiffrement complet de l’appareil. Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 Les **appareils ne parviennent pas à archiver avec le service Intune ou s’affichent comme « défectueux » dans la console d’administration Intune :** Certains appareils Samsung 4,4 et 5,5 ne peuvent pas archiver le service. Il existe trois solutions possibles à ce problème :
  
1. Ouvrez manuellement l’application portail d’entreprise Intune, qui lance automatiquement une synchronisation d’appareil.

2. Mettez à jour l’appareil vers Android 6,0 ou version ultérieure.

3. Désactivez le Gestionnaire intelligent Samsung de la gestion du portail d’entreprise Intune. Consultez [ce document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pour plus d’informations sur ces problèmes et solutions.

 **Type de licence utilisateur non valide** ou **nom d’utilisateur non reconnu :** l’utilisateur doit se voir attribuer une licence Intune ou EMS. Passez en revue ces documents pour attribuer une licence via : Centre d’administration Office ou portail Azure.
  
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants. Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) .

2. Consultez [ce document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pour obtenir la liste des erreurs courantes qui empêchent l’inscription et la résolution de chacune d’elles.

3. [Découvrez comment inscrire des appareils Android dans Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
