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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664924"
---
# <a name="troubleshoot-password-synchronization"></a>Résoudre les problèmes de synchronisation de mot de passe

Pour résoudre les problèmes de synchronisation de mot de passe, commencez par utiliser cette tâche de résolution des problèmes de connexion AAD afin de déterminer pourquoi les mots de passe ne sont pas synchronisés. Pour commencer, accédez à [gérer la synchronisation directe](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD Connect, puis sélectionnez l’option **exécuter en tant qu’administrateur** .

2. Exécuter Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Unrestricted.

3. Démarrez l’Assistant Connexion à Azure AD.

4. Accédez à la page tâches supplémentaires > **résoudre les problèmes**  >  **suivants**.

5. Sélectionnez **lancer** pour ouvrir le menu résolution des problèmes PowerShell.

6. Sélectionnez **résoudre les problèmes de synchronisation de mot de passe**.

    Le problème est généralement dû au fait qu’un mot de passe n’est pas synchronisé pour un compte d’utilisateur spécifique.

    **Remarques** La synchronisation de mot de passe échoue si la dernière synchronisation de mot de passe réussisait quelques instants.

Pour plus d’informations sur la résolution des problèmes de synchronisation de mot de passe, consultez la rubrique [Troubleshoot Password Hash Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).