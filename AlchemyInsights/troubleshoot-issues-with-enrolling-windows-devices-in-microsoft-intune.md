---
title: Résoudre les problèmes liés à l’inscrire des appareils Windows dans Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665830"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Résoudre les problèmes liés à l’inscrire des appareils Windows dans Microsoft Intune

Passez en revue les ressources indiquées ci-dessous pour résoudre votre problème dès maintenant.
  
Les messages d’erreur courants et les étapes de résolution sont les suivants:
  
 **Le logiciel ne peut pas être installé, 0x80cf4017:** Votre certificat de compte a expiré. Téléchargez de nouveau le package logiciel client PC dans la console d’administration Intune. Pour plus d’informations, consultez cette documentation.
  
 **Code d’erreur 0x801c0003:** L’erreur peut se produire dans les scénarios suivants:
  
-  L’utilisateur dispose de plus d’appareils que la limite de l’appareil. Passez en revue ces documents pour [supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou [modifier la limite du périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  «Les utilisateurs peuvent rejoindre les appareils sur Azure AD» est défini sur «aucun». Définissez-la sur tous les utilisateurs ou sélectionnez-les. Pour plus d’informations, consultez [cette documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  L’appareil est déjà déployé par un autre utilisateur. Si c’est le cas, supprimez l’appareil de la console Azure Intune ou désinscrivez manuellement l’appareil, puis réessayez.

-  Le périphérique est Windows 10 Home. Seuls Windows 10 professionnel, les SKU éducation et entreprise peuvent rejoindre Azure Active Directory.

Ressources supplémentaires pour vous aider à résoudre votre problème:
  
-  Utilisez le [portail de résolution des problèmes Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscriptions courants. Pour plus d’informations, consultez [ce document](https://docs.microsoft.com/intune/help-desk-operators) .

-  Consultez ces documents pour obtenir la liste des erreurs courantes qui empêchent l’inscription et la résolution de chacune d’elles: [Guide de dépannage](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [Dépannage doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Découvrez comment inscrire des appareils Windows dans Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
