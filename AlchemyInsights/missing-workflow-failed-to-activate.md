---
title: Échec de l’activation du flux de travail manquant
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543923"
---
# <a name="missing-workflow-failed-to-activate"></a>Échec de l’activation du flux de travail manquant

Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (tel que «approbation-SharePoint 2010») à une liste ou une bibliothèque.
  
Pour résoudre ce problème, procédez comme suit: 
  
1. Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.
  
2. Sous **objets du site**, sélectionnez **flux de travail**. 
  
3. Dans la section **nouveau** du ruban **flux de travail** , sélectionnez **flux**de travail réutilisable. 
  
4. Dans le formulaire **créer un flux de travail** réutilisable, entrez le nom * * *Repair2010* * *. Pour **type de plateforme**, cliquez sur **flux de travail SharePoint 2010**, puis sur **OK**. 
  
1. Dans la section **Enregistrer** du ruban **flux de travail** , sélectionnez **publier**. 
  
2. Dans la section **gérer** du ruban **flux de travail** , sélectionnez **publier globalement**. Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**. 
  
3. Dans un navigateur Web, recherchez le site Web racine de la collection de sites, puis accédez aux **paramètres** \> du site fonctionnalités de la **collection de sites**. Ensuite, activez ou désactivez la fonctionnalité **flux de travail** : 
  
· Si la fonctionnalité est *activée* , cliquez sur désactiver **,** puis sur **activer**. 
  
· Si la fonctionnalité est ** désactivée, cliquez sur **activer**. 
  
Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.
  

