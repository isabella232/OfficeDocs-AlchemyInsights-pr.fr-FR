---
title: Synchronisation des profils
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768111"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quand mon profil modifie-t-il la synchronisation avec l’application de profil utilisateur SharePoint ?

SharePoint Online utilise le travail du minuteur d’importation Active Directory (importation AD) pour importer des utilisateurs et des groupes dans l’application de profil utilisateur. 
  
1. AD Import synchronise les modifications entre le magasin d’annuaires SharePoint Online et l’application de profil utilisateur. Ces modifications sont traitées par lots.
    
2. Le travail du minuteur s’exécute jusqu’à ce que les modifications soient synchronisées.
    
> [!NOTE]
> Le temps nécessaire à l’exécution du travail dépend du nombre de modifications à traiter. Un grand nombre de modifications prend plus de temps. Le contrat de niveau de service (SLA) indique qu’une modification apportée à un utilisateur dans le répertoire SharePoint Online sera reflétée dans l’application de profil utilisateur dans les 24 heures. 
  
[Plus d’informations sur la synchronisation des profils utilisateur dans SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

