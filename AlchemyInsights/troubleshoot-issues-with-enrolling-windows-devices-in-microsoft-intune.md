---
title: Résoudre les problèmes de l’inscription des périphériques Windows Intune Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661526"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Résoudre les problèmes de l’inscription des périphériques Windows Intune Microsoft

Passez en revue les ressources répertoriées ci-dessous pour résoudre le problème maintenant. 
  
Certains messages d’erreur courants et les étapes de résolution :
  
 **Ne peut pas être installé le logiciel, 0x80cf4017 :** Votre certificat de compte a expiré. Télécharger le logiciel PC Client dans la Console d’administration Intune à nouveau. Consultez cette documentation pour plus d’informations. 
  
 **Code d’erreur 0x801c0003 :** L’erreur peut se produire dans les scénarios suivants : 
  
1. L’utilisateur dispose de plusieurs périphériques inscrits à la limite du périphérique. Passez en revue ces documents pour [Supprimer un périphérique](https://docs.microsoft.com/intune/devices-wipe) ou de [Modifier la limite de périphérique](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. « Les utilisateurs peuvent se joindre à périphériques pour Azure AD » est définie sur « none ». Valeur tous ou sélectionnez utilisateurs. Passez en revue [cette documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pour plus d’informations. 
    
3. Le périphérique est déjà inscrit par un autre utilisateur. Si tel est le cas, supprimez le périphérique à partir de la console d’Azure Intune ou unenroll manuellement le périphérique avant de réessayer.
    
4. Le périphérique est 10 d’accueil. Uniquement Windows 10 Pro, formation et SKU peuvent participer à Azure Active Directory.
    
Ressources supplémentaires pour vous aider à résoudre votre problème :
  
1. Utiliser le [Portail de résolution des problèmes de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pour diagnostiquer et résoudre les échecs d’inscription courantes. Passez en revue [ce document](https://docs.microsoft.com/intune/help-desk-operators) pour plus d’informations. 
    
2. Passez en revue ces documents pour la liste des erreurs qui empêchent l’inscription et les résolutions à chacun : [guide de résolution des problèmes](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) et [dépannage doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Apprenez à inscrire des périphériques Windows Intune Microsoft](https://docs.microsoft.com/intune/windows-enroll).
  

