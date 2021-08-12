---
title: La limite quotidienne de courrier électronique a été dépassée. Le flux de travail est suspendu.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914649"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite quotidienne de courrier électronique dépassée. Le flux de travail est suspendu.

Cette erreur peut être reçue dans les scénarios suivants :

- Vous avez un flux de travail dans SharePoint Online qui utilise le type de plateforme de flux de travail SharePoint 2010 ou SharePoint 2013.
- Le flux de travail est configuré pour envoyer un message électronique personnalisé à plus de 200 utilisateurs à la fois, plus de 10 000 destinataires par jour ou plus de 30 messages par minute.
- Lorsque vous exécutez le flux de travail, le message électronique n’est pas envoyé et vous remarquez le comportement suivant :
    - Pour un flux de travail utilisant le type SharePoint 2013, accédez à la page État du flux **de** travail. Dans la page État  du flux de travail, l’état interne est démarré **et** la bulle d’informations affiche Impossible d’envoyer à **un destinataire.**

Pour contourner ce problème, configurez votre flux de travail pour qu’il envoie des messages électroniques sans dépasser [Exchange Online limites de l’expéditeur.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Par exemple, utilisez une pause dans le flux de travail, envoyez le message électronique à un groupe Microsoft 365, à un groupe de distribution ou à un groupe de sécurité à messagerie, ou envoyez le message à moins de 200 destinataires à la fois.


Pour plus d’informations, voir [l’article suivant.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Voir aussi
- [Créer Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint et Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 