---
title: Impossible d’ajouter le flux de travail d’approbation 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748682"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Impossible d’ajouter le flux de travail d’approbation 2010

Dans une collection de sites Microsoft SharePoint, vous ne pouvez pas ajouter un flux de travail réutilisable globalement (tel que « approbation-SharePoint 2010 ») à une liste ou une bibliothèque.
  
Pour résoudre ce problème, procédez comme suit : 
  
1. Ouvrez le site Web racine de la collection de sites dans SharePoint Designer 2013.
  
2. Sous **objets du site**, sélectionnez **flux de travail**. 
  
3. Dans la section **nouveau** du ruban **flux de travail** , sélectionnez flux de travail **réutilisable**. 
  
4. Dans le formulaire **créer un flux de travail réutilisable** , entrez le nom * * *Repair2010* * *. Pour **type de plateforme**, cliquez sur **flux de travail SharePoint 2010**, puis sur **OK**. 
  
1. Dans la section **Enregistrer** du ruban **flux de travail** , sélectionnez **publier**. 
  
2. Dans la section **gérer** du ruban **flux de travail** , sélectionnez **publier globalement**. Dans la boîte de dialogue de confirmation qui s’affiche, sélectionnez **OK**. 
  
3. Dans un navigateur Web, recherchez le site Web racine de la collection de sites, puis accédez aux **paramètres** \> du site fonctionnalités de la **collection de sites**. Activer/désactiver la fonctionnalité **flux de travail** : 
  
· Si la fonctionnalité est *activée* , cliquez sur désactiver **,** puis sur **activer**. 
  
· Si la fonctionnalité est *désactivée* , cliquez sur **activer**. 
  
Pour plus d’informations, reportez-vous à l' [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)suivant.
  

