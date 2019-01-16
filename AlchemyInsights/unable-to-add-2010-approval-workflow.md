---
title: Impossible d’ajouter le flux de travail approbation 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288917"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Impossible d’ajouter le flux de travail approbation 2010

Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (par exemple, « approbation - SharePoint 2010 ») à une liste ou une bibliothèque.
  
Pour résoudre ce problème, procédez comme suit : 
  
1. Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.
  
2. **Objets du Site**, cliquez sur **flux de travail**. 
  
3. Dans la section **Nouveau** du ruban de **flux de travail** , sélectionnez le **Flux de travail réutilisable**. 
  
4. Dans le formulaire de **Flux de travail réutilisable** , entrez le nom ** *Repair2010* **. Pour **Type de plateforme**, cliquez sur **Flux de travail SharePoint 2010**, puis cliquez sur **OK**. 
  
1. Dans la section **Enregistrer** du ruban de **flux de travail** , sélectionnez **Publier**. 
  
2. Dans la section **Gérer** du ruban de **flux de travail** , sélectionnez **Publier globalement**. Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**. 
  
3. Dans un navigateur web, recherchez le site Web racine de la collection de sites, puis accéder aux **Paramètres du Site** \> **Fonctionnalités de Collection de sites**. Activer/désactiver la fonctionnalité de **flux de travail** : 
  
· Si la fonctionnalité est *activé* , cliquez sur **désactiver** et puis cliquez sur **Activer**. 
  
· Si la fonctionnalité est *désactivé* , cliquez sur **Activer**. 
  
Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.
  

