---
title: Résoudre les problèmes liés à l’inscrire des appareils Windows dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658876"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Résoudre les problèmes liés à l’inscrire des appareils Windows dans Microsoft Intune

Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant.
  
Les messages d’erreur courants et les étapes de résolution sont les suivants :
  
 **Le logiciel ne peut pas être installé, 0x80cf4017 :** Votre certificat de compte a expiré. Téléchargez de nouveau le package logiciel client PC dans la console d’administration Intune. Pour plus d’informations, consultez cette documentation.
  
 **Code d’erreur 0x801c0003 :** L’erreur peut se produire dans les scénarios suivants :
  
-  L’utilisateur dispose de plus d’appareils que la limite de l’appareil. Passez en revue ces documents pour [supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou [modifier la limite du périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  « Les utilisateurs peuvent rejoindre les appareils sur Azure AD » est défini sur « aucun ». Définissez-la sur tous les utilisateurs ou sélectionnez-les. Pour plus d’informations, consultez [cette documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  L’appareil est déjà déployé par un autre utilisateur. Si c’est le cas, supprimez l’appareil de la console Azure Intune ou désinscrivez manuellement l’appareil, puis réessayez.

-  Le périphérique est Windows 10 Home. Seuls Windows 10 professionnel, les SKU éducation et entreprise peuvent rejoindre Azure Active Directory.

Ressources supplémentaires pour vous aider à résoudre votre problème :
  
-  Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants. Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) .

-  Consultez ces documents pour obtenir une liste des erreurs courantes qui empêchent l’inscription et les solutions à chacune d’elles : [Guide de résolution des problèmes](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [Résolution des problèmes liés aux documents](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Découvrez comment inscrire des appareils Windows dans Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
