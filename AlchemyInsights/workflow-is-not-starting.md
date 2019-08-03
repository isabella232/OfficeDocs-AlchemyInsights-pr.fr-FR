---
title: Le flux de travail ne démarre pas
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171779"
---
# <a name="workflow-is-not-starting"></a>Le flux de travail ne démarre pas

- Les flux de travail SharePoint 2010 et SharePoint 2013 ne démarrent pas.

    Si votre flux de travail ne démarre pas, il peut y avoir un problème de service temporaire dans lequel les utilisateurs peuvent observer des retards intermittents avec la progression du flux de travail. Consultez le [tableau de bord d’État du service](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pour voir si votre organisation est concernée.

    Si plus de 24 heures se sont écoulées depuis le début de ce problème, veuillez consigner un ticket de support. Dans de nombreux cas, nous travaillons déjà sur une solution. Veuillez nous fournir au moins 24 heures pour terminer une solution.

- Flux de travail SharePoint 2010 retardés au démarrage.

    Cela se produit si le flux de travail est déclenché par des lots volumineux. (par exemple, lorsque plusieurs éléments sont ajoutés à la fois).

    Les flux de travail ne sont pas conçus pour s’exécuter en temps réel, c’est pourquoi un délai est le comportement par défaut.

    Si le flux de travail est complexe Extensible Object Markup Language (XMOL), la compilation peut être lente. Consultez [cet](https://support.microsoft.com/en-us/kb/3043697) article.

    Vous devez simplifier le flux de travail ou le reconcevoir à l’aide du type de plateforme de flux de travail Microsoft SharePoint 2013.

    De plus, si l’historique de vos flux de travail a grandi, vous souhaiterez peut-être purger les éléments ou créer un historique.

    Pour plus d’informations: [purger l’historique du flux de travail](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Sujets associés
Vous souhaitez essayer le flux de test dans SharePoint Online?
- [Créer un flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint et flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


