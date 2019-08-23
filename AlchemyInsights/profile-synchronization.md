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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554331"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5752f-102">Quand mon profil modifie-t-il la synchronisation avec l’application de profil utilisateur SharePoint?</span><span class="sxs-lookup"><span data-stu-id="5752f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5752f-103">SharePoint Online utilise le travail du minuteur d’importation Active Directory (importation AD) pour importer des utilisateurs et des groupes dans l’application de profil utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5752f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5752f-104">AD Import synchronise les modifications entre le magasin d’annuaires SharePoint Online et l’application de profil utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5752f-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="5752f-105">Ces modifications sont traitées par lots.</span><span class="sxs-lookup"><span data-stu-id="5752f-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5752f-106">Le travail du minuteur s’exécute jusqu’à ce que les modifications soient synchronisées.</span><span class="sxs-lookup"><span data-stu-id="5752f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5752f-107">Le temps nécessaire à l’exécution du travail dépend du nombre de modifications à traiter.</span><span class="sxs-lookup"><span data-stu-id="5752f-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="5752f-108">Un grand nombre de modifications prend plus de temps.</span><span class="sxs-lookup"><span data-stu-id="5752f-108">A large number of changes takes longer.</span></span> <span data-ttu-id="5752f-109">Le contrat de niveau de service (SLA) indique qu’une modification apportée à un utilisateur dans le répertoire SharePoint Online sera reflétée dans l’application de profil utilisateur dans les 24 heures.</span><span class="sxs-lookup"><span data-stu-id="5752f-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5752f-110">Plus d’informations sur la synchronisation des profils utilisateur dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5752f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

