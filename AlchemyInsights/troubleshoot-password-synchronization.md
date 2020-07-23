---
title: Résoudre les problèmes de synchronisation de mot de passe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387875"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="2493b-102">Résoudre les problèmes de synchronisation de mot de passe</span><span class="sxs-lookup"><span data-stu-id="2493b-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="2493b-103">Pour résoudre les problèmes de synchronisation de mot de passe, commencez par utiliser cette tâche de résolution des problèmes de connexion AAD afin de déterminer pourquoi les mots de passe ne sont pas synchronisés.</span><span class="sxs-lookup"><span data-stu-id="2493b-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="2493b-104">Pour commencer, accédez à [gérer la synchronisation directe](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="2493b-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="2493b-105">Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD Connect, puis sélectionnez l’option **exécuter en tant qu’administrateur** .</span><span class="sxs-lookup"><span data-stu-id="2493b-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="2493b-106">Exécuter Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="2493b-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="2493b-107">Démarrez l’Assistant Connexion à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2493b-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="2493b-108">Accédez à la page tâches supplémentaires > **résoudre les problèmes**  >  **suivants**.</span><span class="sxs-lookup"><span data-stu-id="2493b-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="2493b-109">Sélectionnez **lancer** pour ouvrir le menu résolution des problèmes PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2493b-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="2493b-110">Sélectionnez **résoudre les problèmes de synchronisation de mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="2493b-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="2493b-111">Le problème est généralement dû au fait qu’un mot de passe n’est pas synchronisé pour un compte d’utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="2493b-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="2493b-112">**Remarques** La synchronisation de mot de passe échoue si la dernière synchronisation de mot de passe réussisait quelques instants.</span><span class="sxs-lookup"><span data-stu-id="2493b-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="2493b-113">Pour plus d’informations sur la résolution des problèmes de synchronisation de mot de passe, consultez la rubrique [Troubleshoot Password Hash Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="2493b-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>