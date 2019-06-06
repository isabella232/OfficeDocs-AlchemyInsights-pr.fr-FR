---
title: Gérer les dictionnaires de recherche dans SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736051"
---
# <a name="search-in-sharepoint-online"></a>Recherche dans SharePoint Online

Le contenu doit être analysé et ajouté à l’index de recherche pour que les utilisateurs puissent trouver ce qu’ils recherchent dans SharePoint Online. Le contenu est automatiquement analysé en fonction d’une planification d’analyse prédéfinie (la planification d’analyse ne peut pas être modifiée). Le robot récupère le contenu qui a été modifié depuis la dernière analyse et met à jour l’index. Pour vous assurer que le contenu est analysé et que l’index est mis à jour, suivez les étapes ci-dessous.

Assurez-vous que le contenu peut être trouvé en effectuant une recherche dans le contenu de site. Pour plus d’informations, consultez [la rubrique activer le contenu sur un site pour pouvoir faire l’objet d’une recherche](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).

Lorsque vous avez modifié une propriété gérée, ou lorsque vous avez modifié le mappage des propriétés analysées et gérées, le site doit être ré-analysé pour que vos modifications soient reflétées dans l’index de recherche. 

Étant donné que vos modifications sont apportées dans le schéma de recherche, et non au site réel, le robot ne réindexe pas automatiquement le site. 

Pour plus d’informations, voir [demander manuellement l’analyse et la réindexation d’un site, d’une bibliothèque ou d’une liste](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).

 Patientez au moins 24 heures après avoir demandé manuellement une analyse et une réindexation complète pour voir si vous rencontrez toujours un problème. 

Si plus de 24 heures se sont écoulées depuis l’ouverture de l’analyse et de la réindexation complète, veuillez consigner un cas de support. Dans de nombreux cas, nous travaillons déjà sur une solution. Veuillez nous fournir au moins 24 heures pour terminer une solution.

**Important**: si un site, un document (bibliothèque) ou une liste a été supprimé et s’affiche toujours dans les résultats de la recherche, les utilisateurs doivent recevoir un fichier d’erreur 404 introuvable lors de la tentative d’accès. Ce problème doit être consigné dans le cadre d’une demande d’assistance supplémentaire. 



