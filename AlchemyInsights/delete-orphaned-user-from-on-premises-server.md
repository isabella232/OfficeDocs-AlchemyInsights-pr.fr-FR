---
title: Supprimer l’utilisateur orphelin du serveur local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186107"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="98ffc-102">Supprimer l’utilisateur orphelin du serveur local</span><span class="sxs-lookup"><span data-stu-id="98ffc-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="98ffc-103">Pour supprimer un utilisateur orphelin, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="98ffc-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="98ffc-104">Forcer la synchronisation d’annuaires en suivant les instructions dans [Qu’est-ce que l’identité hybride avec Azure Active Directory ?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="98ffc-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="98ffc-105">Pour vérifier la synchronisation d’annuaires, consultez [Qu’est-ce que l’identité hybride avec Azure Active Directory ?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="98ffc-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="98ffc-106">Si la synchronisation fonctionne correctement, mais que la suppression d’objets Active Directory ne se propage pas à Azure AD, supprimez manuellement l’objet orphelin à l’aide de l’un des applets de commande Module Azure Active Directory pour Windows PowerShell :</span><span class="sxs-lookup"><span data-stu-id="98ffc-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="98ffc-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="98ffc-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="98ffc-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="98ffc-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="98ffc-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="98ffc-109">Remove-MsolUser</span></span>

    <span data-ttu-id="98ffc-110">Par exemple, pour supprimer l’ID utilisateur orphelin john.smith@contoso.com, créé à l’origine à l’aide de la synchronisation d’annuaires, exécutez l’applet de commande :</span><span class="sxs-lookup"><span data-stu-id="98ffc-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="98ffc-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="98ffc-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>