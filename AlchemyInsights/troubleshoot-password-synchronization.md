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
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="ee1b8-102">Résoudre les problèmes de synchronisation de mot de passe</span><span class="sxs-lookup"><span data-stu-id="ee1b8-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="ee1b8-103">Pour résoudre les problèmes où aucun mot de passe n’est synchronisés avec Azure AD Connect version 1.1.614.0 ou version ultérieure :</span><span class="sxs-lookup"><span data-stu-id="ee1b8-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="ee1b8-104">Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD se connecter avec l’option **Exécuter en tant qu’administrateur** .</span><span class="sxs-lookup"><span data-stu-id="ee1b8-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="ee1b8-105">Exécutez **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="ee1b8-106">Démarrez l’Assistant Azure AD se connecter.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="ee1b8-107">Accédez à la \*\* tâches supplémentaires \*\* page, sélectionnez \*\* Troubleshoot \*\*, puis cliquez sur **suivant**.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="ee1b8-108">Dans la page de résolution des problèmes, cliquez sur le menu de **lancement pour démarrer la résolution des problèmes** dans PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="ee1b8-109">Dans le menu principal, sélectionnez **Résoudre les problèmes de synchronisation de mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="ee1b8-110">Dans le menu sub, activez **la synchronisation de mot de passe ne fonctionne pas du tout**.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="ee1b8-111">**Comprendre les résultats de la tâche de résolution des problèmes**</span><span class="sxs-lookup"><span data-stu-id="ee1b8-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="ee1b8-112">La tâche de résolution des problèmes des vérifications suivantes :</span><span class="sxs-lookup"><span data-stu-id="ee1b8-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="ee1b8-113">Vérifie que la fonctionnalité de synchronisation de mot de passe est activée pour votre client Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="ee1b8-114">Vérifie que le serveur de Azure AD Connect n’est pas en mode de mise en attente.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="ee1b8-115">Pour chaque connecteur local Active Directory existant (qui correspond à une forêt Active Directory existante) :</span><span class="sxs-lookup"><span data-stu-id="ee1b8-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="ee1b8-116">Vérifie que la fonctionnalité de synchronisation de mot de passe est activée.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="ee1b8-117">Recherche les événements de pulsation la synchronisation de mot de passe dans les journaux des événements d’applications Windows.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="ee1b8-118">Pour chaque domaine Active Directory sous le connecteur Active Directory local :</span><span class="sxs-lookup"><span data-stu-id="ee1b8-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="ee1b8-119">Vérifie que le domaine est accessible à partir du serveur Azure AD se connecter.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="ee1b8-120">Valide le fait que les comptes de Services de domaine Active Directory (AD DS) utilisés par le connecteur Active Directory local possède le nom d’utilisateur correct, le mot de passe et les autorisations requises pour la synchronisation de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="ee1b8-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="ee1b8-121">Pour plus d’aide Résolution des problèmes de synchronisation de mot de passe, voir [Troubleshoot la synchronisation de mot de passe avec la synchronisation Azure Active Directory se connecter](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ee1b8-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

