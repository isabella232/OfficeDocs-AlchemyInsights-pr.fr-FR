---
title: Synchronisation des profils
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920086"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="ffa9f-102">Lorsque les modifications du profil synchroniser à l’Application de profil utilisateur SharePoint ?</span><span class="sxs-lookup"><span data-stu-id="ffa9f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="ffa9f-103">SharePoint Online utilise le travail du minuteur importation Active Directory (importation AD) pour importer les utilisateurs et les groupes dans l’Application de profil utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ffa9f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="ffa9f-p101">L’importation AD de synchroniser les modifications dans le magasin d’annuaire SharePoint Online à l’Application de profil utilisateur. Ces modifications sont traitées par lots.</span><span class="sxs-lookup"><span data-stu-id="ffa9f-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="ffa9f-106">Le travail du minuteur s’exécute jusqu'à ce que les modifications sont synchronisées.</span><span class="sxs-lookup"><span data-stu-id="ffa9f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="ffa9f-p102">Le temps que nécessaire à l’exécution du travail varie selon le nombre de modifications à traiter. Un grand nombre de modifications prend plus de temps. Le contrat de niveau de Service (SLA) indique une modification apportée à un utilisateur dans SharePoint Online Directory est reflétée dans l’Application de profil utilisateur dans les 24 heures.</span><span class="sxs-lookup"><span data-stu-id="ffa9f-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="ffa9f-110">Plus d’informations sur la synchronisation de profil utilisateur dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ffa9f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

