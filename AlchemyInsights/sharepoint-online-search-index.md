---
title: Recherche dans SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507629"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Analyse et indexation de contenu dans SharePoint Online

Le contenu doit être analysé et ajouté à l’index de recherche pour que les utilisateurs puissent trouver ce qu’ils recherchent dans SharePoint Online. Le contenu est automatiquement analysé en fonction d’une planification d’analyse prédéfinie (la planification d’analyse ne peut pas être modifiée). Le robot récupère le contenu qui a été modifié depuis la dernière analyse et met à jour l’index. Pour vous assurer que le contenu est analysé et que l’index est mis à jour, notez les points suivants:

- Assurez-vous que le contenu peut être trouvé en effectuant une recherche dans le [contenu de site](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Lorsque vous avez modifié une propriété gérée, ou lorsque vous avez modifié le mappage des propriétés analysées et gérées, le site doit être ré-analysé pour que vos modifications soient reflétées dans l’index de recherche. 

    Étant donné que vos modifications sont apportées dans le schéma de recherche, et non au site réel, le robot ne réindexe pas automatiquement le site. 

    Pour plus d’informations, voir [demander manuellement l’analyse et la réindexation d’un site, d’une bibliothèque ou d’une liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Patientez au moins 24 heures après avoir demandé manuellement une analyse et une réindexation complète pour voir si vous rencontrez toujours un problème. 

    Si plus de 24 heures se sont écoulées depuis l’ouverture de l’analyse et de la réindexation complète, veuillez consigner un cas de support. Dans de nombreux cas, nous travaillons déjà sur une solution. Veuillez nous fournir au moins 24 heures pour terminer une solution.

> [!IMPORTANT]
> Si un site, un document (bibliothèque) ou une liste a été supprimé et s’affiche toujours dans les résultats de la recherche, les utilisateurs doivent recevoir une **erreur 404 fichier** introuvable lors de la tentative d’accès. Ce problème doit être consigné dans le cadre d’une demande d’assistance supplémentaire. 



