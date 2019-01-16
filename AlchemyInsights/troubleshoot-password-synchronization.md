---
title: Résoudre les problèmes de synchronisation de mot de passe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288490"
---
# <a name="troubleshoot-password-synchronization"></a>Résoudre les problèmes de synchronisation de mot de passe

Pour résoudre les problèmes où aucun mot de passe n’est synchronisés avec Azure AD Connect version 1.1.614.0 ou version ultérieure :
  
1. Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD se connecter avec l’option **Exécuter en tant qu’administrateur** . 
    
2. Exécutez **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy Unrestricted**. 
    
3. Démarrez l’Assistant Azure AD se connecter.
    
4. Accédez à la ** tâches supplémentaires ** page, sélectionnez ** Troubleshoot **, puis cliquez sur **suivant**. 
    
5. Dans la page de résolution des problèmes, cliquez sur le menu de **lancement pour démarrer la résolution des problèmes** dans PowerShell. 
    
6. Dans le menu principal, sélectionnez **Résoudre les problèmes de synchronisation de mot de passe**. 
    
7. Dans le menu sub, activez **la synchronisation de mot de passe ne fonctionne pas du tout**. 
    
 **Comprendre les résultats de la tâche de résolution des problèmes**
  
La tâche de résolution des problèmes des vérifications suivantes :
  
- Vérifie que la fonctionnalité de synchronisation de mot de passe est activée pour votre client Azure AD.
    
- Vérifie que le serveur de Azure AD Connect n’est pas en mode de mise en attente.
    
- Pour chaque connecteur local Active Directory existant (qui correspond à une forêt Active Directory existante) :
    
- 
  - Vérifie que la fonctionnalité de synchronisation de mot de passe est activée.
    
  - Recherche les événements de pulsation la synchronisation de mot de passe dans les journaux des événements d’applications Windows.
    
  - Pour chaque domaine Active Directory sous le connecteur Active Directory local :
    
  - Vérifie que le domaine est accessible à partir du serveur Azure AD se connecter.
    
  - Valide le fait que les comptes de Services de domaine Active Directory (AD DS) utilisés par le connecteur Active Directory local possède le nom d’utilisateur correct, le mot de passe et les autorisations requises pour la synchronisation de mot de passe.
    
Pour plus d’aide Résolution des problèmes de synchronisation de mot de passe, voir [Troubleshoot la synchronisation de mot de passe avec la synchronisation Azure Active Directory se connecter](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

