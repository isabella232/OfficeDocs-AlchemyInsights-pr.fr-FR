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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390419"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="50a58-102">Résoudre les problèmes de synchronisation de mot de passe</span><span class="sxs-lookup"><span data-stu-id="50a58-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="50a58-103">Pour résoudre les problèmes où aucun mot de passe n'est synchronisé avec Azure AD Connect version 1.1.614.0 ou ultérieure:</span><span class="sxs-lookup"><span data-stu-id="50a58-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="50a58-104">Ouvrez une nouvelle session Windows PowerShell sur votre serveur Azure AD Connect avec l'option **exécuter en tant qu'administrateur** .</span><span class="sxs-lookup"><span data-stu-id="50a58-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="50a58-105">Exécuter **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="50a58-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="50a58-106">Démarrez l'Assistant Connexion à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50a58-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="50a58-107">Accédez à la page \* \* autres tâches \* \*, sélectionnez \* \* Troubleshooting \* \*, puis cliquez sur **suivant**.</span><span class="sxs-lookup"><span data-stu-id="50a58-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="50a58-108">Sur la page résolution des problèmes, cliquez sur démarrer **pour démarrer le menu dépannage** dans PowerShell.</span><span class="sxs-lookup"><span data-stu-id="50a58-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="50a58-109">Dans le menu principal, sélectionnez **résoudre les problèmes de synchronisation de mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="50a58-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="50a58-110">Dans le sous-menu, sélectionnez la **synchronisation de mot de passe ne fonctionne pas du tout**.</span><span class="sxs-lookup"><span data-stu-id="50a58-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="50a58-111">**Comprendre les résultats de la tâche de résolution des problèmes**</span><span class="sxs-lookup"><span data-stu-id="50a58-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="50a58-112">La tâche de résolution des problèmes effectue les vérifications suivantes:</span><span class="sxs-lookup"><span data-stu-id="50a58-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="50a58-113">Vérifie que la fonctionnalité de synchronisation de mot de passe est activée pour votre client Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50a58-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="50a58-114">Vérifie que le serveur Azure AD Connect n'est pas en mode intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="50a58-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="50a58-115">Pour chaque connecteur Active Directory local existant (ce qui correspond à une forêt Active Directory existante):</span><span class="sxs-lookup"><span data-stu-id="50a58-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="50a58-116">Vérifie que la fonctionnalité de synchronisation de mot de passe est activée.</span><span class="sxs-lookup"><span data-stu-id="50a58-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="50a58-117">Recherche les événements de pulsation de synchronisation de mot de passe dans les journaux d'événements d'applications Windows.</span><span class="sxs-lookup"><span data-stu-id="50a58-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="50a58-118">Pour chaque domaine Active Directory sous le connecteur Active Directory local:</span><span class="sxs-lookup"><span data-stu-id="50a58-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="50a58-119">Vérifie que le domaine est accessible à partir du serveur Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="50a58-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="50a58-120">Vérifie que les comptes des services de domaine Active Directory (AD DS) utilisés par le connecteur Active Directory local possèdent le nom d'utilisateur, le mot de passe et les autorisations appropriés pour la synchronisation de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="50a58-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="50a58-121">Pour plus d'informations sur la résolution des problèmes de synchronisation de mot de passe, consultez la rubrique [Troubleshoot Password Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="50a58-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

