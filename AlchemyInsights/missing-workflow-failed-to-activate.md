---
title: Échec de l’activation du flux de travail manquant
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065426"
---
# <a name="missing-workflow-failed-to-activate"></a>Échec de l’activation du flux de travail manquant

Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (tel que « Approbation - SharePoint 2010 ») à une liste ou une bibliothèque.
  
Pour résoudre ce problème, suivez les étapes suivantes : 
  
1. Ouvrez le site web racine de la collection de sites dans SharePoint Designer 2013.
  
2. Sous **Objets du site,** sélectionnez **Flux de travail.** 
  
3. Dans la **section Nouveau** du ruban **Flux** de travail, sélectionnez Flux de **travail réutilisable.** 
  
4. Dans le **formulaire Créer un flux de** travail réutilisable, entrez le nom ** *Repair2010* **. Pour **type de plateforme,** cliquez SharePoint flux de **travail 2010,** puis cliquez sur **OK**. 
  
1. Dans la section **Enregistrer** du ruban **flux de** travail, sélectionnez **Publier.** 
  
2. Dans la section **Gérer** du ruban **Flux de** travail, **sélectionnez Publier globalement.** Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK.** 
  
3. Dans un navigateur web, recherchez le site web  racine de la collection de sites, puis accédez aux fonctionnalités Paramètres \> **collection de sites.** Ensuite, basculez la fonctionnalité **Flux de** travail : 
  
· Si la fonctionnalité est *activée,* cliquez **sur Désactiver,** puis sur **Activer.** 
  
· Si la fonctionnalité est *désactivée,* cliquez sur **Activer.** 
  
Pour plus d’informations, reportez-vous à [l’article suivant.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

