---
title: Le courrier électronique de flux de travail n’est pas envoyé
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049371"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Le courrier de flux de travail n’est pas envoyé pour une liste ou une bibliothèque SharePoint

1. Les courriers électroniques provenant de flux de travail ne sont pas envoyés à tous les utilisateurs ou uniquement à des utilisateurs spécifiques, ou vous voyez l’erreur que **le message électronique ne peut pas être envoyé. Assurez-vous que le message électronique contient un destinataire valide**.

    Vérifiez si l’utilisateur existe dans le groupe d’autorisations **tous les personnes** (liste d’informations utilisateur) pour cette collection de sites.  Exemple d’URL directe :<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx ? MembershipGroupId = 0

    - Si l’utilisateur n’existe pas, vérifiez que l’utilisateur est connecté à la page. 
    - S’il s’agit d’un utilisateur externe, assurez-vous que son invitation a été acceptée.
    - Si l’utilisateur existe dans le groupe d’autorisations, assurez-vous que l’adresse de messagerie est correcte.
    - Si l’adresse de messagerie de l’utilisateur n’est pas définie ici, créez un exemple d’alerte pour cet utilisateur, ce qui force la synchronisation de ce compte d’utilisateur à partir des profils utilisateur de SharePoint vers cette collection de sites.
 
2. Les courriers électroniques provenant de flux de travail sont envoyés aux administrateurs de collection de sites, mais pas aux autres utilisateurs et le message d’erreur **http interdit à <span>https :</span>//URL/_vti_bin/client.XVC.sp.Utilities.Utility.SendEmail**.
 

    Consultez [la rubrique accès refusé lorsque vous envoyez un message électronique à un groupe SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Vérifiez également que la fonctionnalité de collection de sites **mode verrouillage avec accès limité aux utilisateurs** n’est pas active.


## <a name="related-topics"></a>Voir aussi
Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?
- [Créer un flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint et flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


