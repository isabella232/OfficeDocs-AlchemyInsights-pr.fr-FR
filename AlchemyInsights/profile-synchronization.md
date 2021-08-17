---
title: Synchronisation des profils
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320707"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quand les modifications apportées à mon profil sont-elles synchronisées avec l SharePoint’application de profil utilisateur ?

SharePoint Online utilise le travail du timer d’importation Active Directory (importation AD) pour importer des utilisateurs et des groupes dans l’application de profil utilisateur. 
  
1. L’importation AD synchronise les modifications du SharePoint d’annuaire en ligne vers l’application de profil utilisateur. Ces modifications sont traitées par lots.
    
2. Le travail du timer s’exécute jusqu’à ce que les modifications soient synchronisées.
    
**Remarque**: le temps d’exécuter le travail dépend du nombre de modifications à traiter. Un grand nombre de modifications prend plus de temps. Le contrat de niveau de service (SLA) indique qu’une modification d’un utilisateur dans l’annuaire SharePoint Online sera reflétée dans l’application de profil utilisateur dans les 24 heures. 
  
[Plus d’informations sur la synchronisation des profils utilisateur dans SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

