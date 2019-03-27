---
title: Résoudre les problèmes de synchronisation de mot de passe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767174"
---
# <a name="troubleshoot-password-synchronization"></a>Résoudre les problèmes de synchronisation de mot de passe

Pour résoudre les problèmes où aucun mot de passe n'est synchronisé avec Azure AD Connect version 1.1.614.0 ou ultérieure:
  
1. Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD Connect avec l'option **exécuter en tant qu'administrateur** . 
    
2. Exécuter **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy Unrestricted**. 
    
3. Démarrez l'Assistant Connexion à Azure AD.
    
4. Accédez à la page * * autres tâches * *, sélectionnez * * Troubleshooting * *, puis cliquez sur **suivant**. 
    
5. Sur la page résolution des problèmes, cliquez sur démarrer **pour démarrer le menu dépannage** dans PowerShell. 
    
6. Dans le menu principal, sélectionnez **résoudre les problèmes de synchronisation de mot de passe**. 
    
7. Dans le sous-menu, sélectionnez la **synchronisation de mot de passe ne fonctionne pas du tout**. 
    
 **Comprendre les résultats de la tâche de résolution des problèmes**
  
La tâche de résolution des problèmes effectue les vérifications suivantes:
  
- Vérifie que la fonctionnalité de synchronisation de mot de passe est activée pour votre client Azure AD.
    
- Vérifie que le serveur Azure AD Connect n'est pas en mode intermédiaire.
    
- Pour chaque connecteur Active Directory local existant (ce qui correspond à une forêt Active Directory existante):
    
- 
  - Vérifie que la fonctionnalité de synchronisation de mot de passe est activée.
    
  - Recherche les événements de pulsation de synchronisation de mot de passe dans les journaux d'événements d'applications Windows.
    
  - Pour chaque domaine Active Directory sous le connecteur Active Directory local:
    
  - Vérifie que le domaine est accessible à partir du serveur Azure AD Connect.
    
  - Vérifie que les comptes des services de domaine Active Directory (AD DS) utilisés par le connecteur Active Directory local possèdent le nom d'utilisateur, le mot de passe et les autorisations appropriés pour la synchronisation de mot de passe.
    
Pour plus d'informations sur la résolution des problèmes de synchronisation de mot de passe, consultez la rubrique [Troubleshoot Password Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

