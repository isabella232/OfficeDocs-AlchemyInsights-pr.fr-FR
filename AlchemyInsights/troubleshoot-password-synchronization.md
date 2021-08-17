---
title: Résoudre les problèmes de synchronisation de mot de passe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105747"
---
# <a name="troubleshoot-password-synchronization"></a>Résoudre les problèmes de synchronisation de mot de passe

Pour résoudre les problèmes de synchronisation des mots de passe, commencez par utiliser cette tâche de résolution des Connecter AAD pour déterminer pourquoi les mots de passe ne sont pas synchronisés. Pour commencer, allez à [Gérer la synchronisation directe.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD Connecter, puis sélectionnez l’option Exécuter **en tant qu’administrateur.**

2. Exécutez Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Unrestricted.

3. Démarrez l’Assistant Connecter Azure AD.

4. Go to the Additional Tasks page > **Troubleshoot**  >  **Next**.

5. Sélectionnez **Lancer** pour ouvrir le menu de dépannage de PowerShell.

6. Sélectionnez **Résoudre les problèmes de synchronisation de mot de passe.**

    Le problème est généralement qu’un mot de passe n’est pas synchronisé pour un compte d’utilisateur spécifique.

    **Remarques** La synchronisation de mot de passe échoue si la dernière synchronisation de mot de passe réussie a eu un certain temps.

Pour plus d’informations sur la résolution des problèmes de synchronisation de mot de passe, voir Résoudre les problèmes de synchronisation de hachage de mot de passe avec [Azure AD Connecter synchronisation.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)