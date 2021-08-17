---
title: Le courrier électronique de flux de travail n’est pas envoyé
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
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072518"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Le courrier électronique de flux de travail n’est pas envoyé pour SharePoint liste ou bibliothèque

1. Les messages électroniques provenant de flux de travail ne sont pas envoyés à tous les utilisateurs ou uniquement à des utilisateurs spécifiques, ou vous voyez l’erreur Le message électronique ne peut pas être **envoyé. Assurez-vous** que le message électronique a un destinataire valide.

    Vérifiez si l’utilisateur existe dans **le** groupe d’autorisations Toutes les personnes (liste d’informations utilisateur) pour cette collection de sites.  Exemple d’URL directe : https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx ? MembershipGroupId=0

    - Si l’utilisateur n’existe pas, assurez-vous qu’il est bien inscrit sur la page. 
    - S’il s’agit d’un utilisateur externe, assurez-vous que son invitation a été acceptée.
    - Si l’utilisateur existe dans le groupe d’autorisations, assurez-vous que l’adresse e-mail est correcte.
    - Si l’adresse de messagerie des utilisateurs n’est pas définie ici, créez un exemple d’alerte pour cet utilisateur qui force la synchronisation de ce compte d’utilisateur à partir des profils utilisateur de SharePoint vers cette collection de sites.
 
2. Les courriers électroniques provenant de flux de travail sont envoyés aux administrateurs de collection de sites, mais pas aux autres utilisateurs et l’erreur HTTP Interdit à **<span>https:</span>//URL/_vti_bin/client.domainedess.sp.utilities.utility.SendEmail**.
 

    Voir [Accès refusé lorsque vous envoyez un e-mail à un SharePoint groupe.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Vérifiez également que la fonctionnalité de collection de sites en **mode** verrouillage des autorisations utilisateur à accès limité n’est pas active.


## <a name="related-topics"></a>Voir aussi
Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?
- [Créer Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint et Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


