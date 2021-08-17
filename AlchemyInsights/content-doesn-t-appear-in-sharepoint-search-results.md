---
title: Le contenu n’apparaît pas dans les résultats SharePoint recherche
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
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081608"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Le contenu n’apparaît pas dans les résultats SharePoint recherche

Suivez ces étapes de dépannage lorsque le contenu attendu n’apparaît pas dans les résultats de la recherche :
  
1. Vérifiez que le **site qui** contient le contenu attendu est définie pour autoriser l’apparition du contenu dans les résultats de la recherche. Suivez les étapes de [l’étape Afficher le contenu sur un site dans les résultats de la recherche.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Vérifiez que la **liste ou** la **bibliothèque** qui contient le contenu attendu est définie pour autoriser l’apparition du contenu dans les résultats de la recherche. Suivez les étapes de [l’étape Afficher le contenu à partir de listes ou de bibliothèques dans les résultats de recherche.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Vérifiez que la page, le document ou la mise en page personnalisée est publié en tant que **version Majeure.** Suivez l’étape 3 de la recherche ne retourne pas tous les résultats [dans SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Vérifiez que l’utilisateur dispose **des autorisations pour** afficher le contenu. Suivez les étapes de [La compréhension des niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Si le schéma de recherche a été modifié par l’ajout d’une nouvelle propriété gérée, la modification d’une propriété gérée ou la suppression d’une propriété gérée, la demande d’une analyse et d’une nouvelle indexation sera nécessaire. **Ré-indexez** le contenu en suivant les étapes de demande manuelle d’analyse et de ré-indexation d’un site, d’une [bibliothèque ou d’une liste.](https://docs.microsoft.com/sharepoint/crawl-site-content) Cela peut prendre un certain temps, patienter 24 heures avant de vérifier à nouveau les résultats.

Pour plus d’informations, voir Activer la recherche de contenu [sur un site.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
