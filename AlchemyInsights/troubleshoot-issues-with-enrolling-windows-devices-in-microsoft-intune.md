---
title: Résoudre les problèmes d'inscription d'appareils Windows dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808969"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Résoudre les problèmes d'inscription d'appareils Windows dans Microsoft Intune

Examinez les ressources répertoriées ci-dessous pour résoudre votre problème maintenant.
  
Voici quelques messages d'erreur courants et les étapes de résolution :
  
 **Le logiciel ne peut pas être installé, 0x80cf4017 :** Le certificat de votre compte a expiré. Téléchargez à nouveau le package logiciel client PC dans la console d'administration Intune. Pour plus d'informations, examinez cette documentation.
  
 **Code d'0x801c0003 :** L'erreur peut se produire dans les scénarios suivants :
  
-  L'utilisateur a plus d'appareils inscrits que la limite d'appareils. Examinez ces documents pour [supprimer un appareil ou](https://docs.microsoft.com/intune/devices-wipe) modifier la limite de [l'appareil.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  « Les utilisateurs peuvent joindre des appareils à Azure AD » est définie sur « aucun ». Définissez-la sur tous les utilisateurs ou sélectionnez-les. Pour plus [d'informations,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) examinez cette documentation.

-  L'appareil est déjà inscrit par un autre utilisateur. Si c'est le cas, supprimez l'appareil de la console Azure Intune ou désinscrissez manuellement l'appareil avant d'essayer à nouveau.

-  L'appareil est Windows 10 Famille. Seules les SSO Windows 10 Professionnel, Éducation et Entreprise peuvent rejoindre Azure Active Directory.

Ressources supplémentaires pour vous aider à résoudre votre problème :
  
-  Utilisez [le portail de dépannage Intune pour](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostiquer et résoudre les échecs d'inscription courants. Pour [plus d'informations,](https://docs.microsoft.com/intune/help-desk-operators) examinez ce document.

-  Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Découvrez comment inscrire des appareils Windows dans Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
