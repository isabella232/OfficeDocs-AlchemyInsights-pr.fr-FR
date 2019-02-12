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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Lorsque les modifications du profil synchroniser à l’Application de profil utilisateur SharePoint ?

SharePoint Online utilise le travail du minuteur importation Active Directory (importation AD) pour importer les utilisateurs et les groupes dans l’Application de profil utilisateur. 
  
1. L’importation AD de synchroniser les modifications dans le magasin d’annuaire SharePoint Online à l’Application de profil utilisateur. Ces modifications sont traitées par lots.
    
2. Le travail du minuteur s’exécute jusqu'à ce que les modifications sont synchronisées.
    
> [!NOTE]
> Le temps que nécessaire à l’exécution du travail varie selon le nombre de modifications à traiter. Un grand nombre de modifications prend plus de temps. Le contrat de niveau de Service (SLA) indique une modification apportée à un utilisateur dans SharePoint Online Directory est reflétée dans l’Application de profil utilisateur dans les 24 heures. 
  
[Plus d’informations sur la synchronisation de profil utilisateur dans SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

