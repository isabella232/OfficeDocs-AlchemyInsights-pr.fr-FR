---
title: Le contenu n’apparaît pas dans les résultats de la recherche SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713128"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Le contenu n’apparaît pas dans les résultats de la recherche SharePoint

Suivez ces étapes de résolution des problèmes lorsque le contenu attendu n’apparaît pas dans les résultats de la recherche :
  
1. Vérifiez que le **site** qui contient le contenu attendu est défini pour autoriser le contenu à apparaître dans les résultats de la recherche. Suivez les étapes décrites dans [afficher le contenu d’un site dans les résultats de la recherche](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Vérifiez que la **liste** ou la **bibliothèque** qui contient le contenu attendu est définie pour autoriser le contenu à apparaître dans les résultats de la recherche. Suivez les étapes de la procédure [afficher le contenu de listes ou de bibliothèques dans les résultats](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)de la recherche.

3. Vérifiez que la page, le document ou la mise en page personnalisée est publié en tant que **version majeure.** Suivez l’étape 3 dans la [recherche ne renvoie pas tous les résultats dans SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Vérifiez que l’utilisateur dispose des **autorisations nécessaires** pour afficher le contenu. Suivez les étapes de [Présentation des niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Si le schéma de recherche a été modifié par l’ajout d’une nouvelle propriété gérée, par la modification d’une propriété gérée ou par la suppression d’une propriété gérée, une demande d’analyse et de réindexement sera requise. **Réindexer** le contenu en suivant les étapes de la procédure de [demande d’analyse et de réindexation manuelle d’un site, d’une bibliothèque ou d’une liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Cette opération peut prendre un certain temps, attendre 24 heures avant de vérifier à nouveau les résultats.

Pour plus d’informations, consultez [la rubrique activer le contenu d’un site pour pouvoir faire l’objet d’une recherche](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
