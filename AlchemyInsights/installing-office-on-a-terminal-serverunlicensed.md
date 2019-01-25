---
title: L’installation d’office sur un serveur Terminal Server - sans licence
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468891"
---
# <a name="installing-office-on-a-terminal-server"></a>Installez Office sur un serveur Terminal Server

Pour le déploiement d’Office 365 ProPlus sur un serveur Windows à l’aide de Remote Desktop Services (RDS), anciennement Services Terminal Server :
  
- Vous devez disposer d’un plan Office 365 qui inclut Office 365 ProPlus, telles que Office 365 entreprise E3 ou entreprise E5. Les plans Office 365 entreprise et Office 365 entreprise Premium n’incluent pas Office 365 ProPlus.
    
- Vous devez activer [l’activation de l’ordinateur partagé](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Si vous souhaitez installer Office 365 ProPlus à partir du portail Office 365, sur RDS ** *qui utilise les paramètres d’installation par défaut* **, procédez comme suit : 
  
1. Vérifier quels plan Office 365 que vous avez. [Découvrez comment](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Si nécessaire, basculez vers un autre Office 365 planifier. [Découvrez comment](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Si Office est déjà installé sur le serveur RDS à l’aide de tous les autres plans Office 365, désinstallez-la. Par exemple, en accédant au panneau \> désinstaller un programme. Désinstallation à l’aide de [l’Assistant de récupération et de prise en charge de Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous utilisez des problèmes. 
    
4. Sur le serveur RDS, connectez-vous au portail Office 365 avec votre compte d’administrateur et [installez Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Une fois Office est installé, ** *ne pas ouvrir ou connectez-vous* ** pour toutes les applications Office. 
    
6. Sur le serveur RDS, activer un ordinateur partagé en modifiant le Registre en procédant comme suit :
    
1. Cliquez sur le bouton Windows dans l’angle inférieur gauche de votre écran, puis sélectionnez Exécuter. Dans la zone Ouvrir, tapez **regedit**, puis sélectionnez OK. 
    
2. Sélectionnez Oui lorsque vous êtes invité à autoriser l’Éditeur du Registre pour apporter des modifications à votre appareil.
    
3. Dans l’Éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec la valeur 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Sur le serveur RDS, ** *se connecter en tant qu’un utilisateur final* ** et [Vérifiez que l’activation de l’ordinateur partagé est activé pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Pour plus d’informations sur les conditions préalables, des instructions d’installation et des conseils sur les installations personnalisées à l’aide de l’outil de déploiement d’Office, consultez [Déploiement d’Office 365 ProPlus à l’aide des Services Bureau à distance](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Pour corriger les erreurs liées à l’activation de l’ordinateur partagé, consultez [résoudre les problèmes liés à l’activation d’un ordinateur partagé pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

