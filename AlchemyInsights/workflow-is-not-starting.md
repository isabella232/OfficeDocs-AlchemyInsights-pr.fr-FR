---
title: Le flux de travail ne démarre pas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907736"
---
# <a name="workflow-is-not-starting"></a>Le flux de travail ne démarre pas

- SharePoint flux de travail 2010 SharePoint 2013 ne démarrent pas.

    - Si votre flux de travail ne démarre pas, il peut y avoir un problème de service temporaire dans lequel les utilisateurs peuvent faire face à des retards intermittents avec la progression du flux de travail. Consultez le [tableau de bord d’état](https://admin.microsoft.com/AdminPortal/Home/servicehealth) du service pour voir si votre organisation est impactée.

    - Si plus de 24 heures se sont écoulées depuis le premier problème, veuillez enregistrer un ticket de support. Dans de nombreux cas, nous travaillons déjà sur une solution. Veuillez nous donner au moins 24 heures pour terminer une solution.

- SharePoint flux de travail 2010 retardés au démarrage.

    - Cela se produit si le flux de travail est déclenché par lots importants. (par exemple, lorsque plusieurs éléments sont ajoutés en même temps).

    - Les flux de travail ne sont pas conçus pour s’exécuter en temps réel. Un délai est donc un comportement par conception.

   -  Si le flux de travail est un langage X WORKFLOW (Extensible Object Markup Language) complexe, la compilation peut être lente. Consultez [cet](https://support.microsoft.com//kb/3043697) article.

    - Vous devez simplifier le flux de travail ou le reconçre à l’aide du type de plateforme de flux de travail Microsoft SharePoint 2013.

    - Si l’historique de votre flux de travail est devenu important, vous pouvez vider les éléments ou créer une liste d’historique.

        Plus d’informations : [Purger l’historique des flux de travail](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Voir aussi
Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?
- [Créer Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint et Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
