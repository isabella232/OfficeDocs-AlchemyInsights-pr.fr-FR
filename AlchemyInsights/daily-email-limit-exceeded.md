---
title: Limite de messagerie quotidienne dépassée. Le flux de travail est suspendu.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514448"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite de messagerie quotidienne dépassée. Le flux de travail est suspendu.

Cette erreur peut être reçue dans les scénarios suivants:

- Vous disposez d’un flux de travail dans SharePoint Online qui utilise le type de plateforme de flux de travail SharePoint 2010 ou SharePoint 2013.
- Le flux de travail est configuré pour envoyer un message électronique personnalisé à plus de 200 utilisateurs à la fois, plus de 10 000 destinataires par jour ou plus de 30 messages par minute.
- Lorsque vous exécutez le flux de travail, le message électronique n’est pas envoyé et vous remarquez le comportement suivant:
    - Pour un flux de travail qui utilise le type de plateforme SharePoint 2013, accédez à la page **État du flux de travail** . Dans la page État du flux de travail, le **statut interne** est défini sur **démarré**, et la bulle d’informations affiche **Impossible d’envoyer à un destinataire**.

Pour contourner ce problème, configurez votre flux de travail pour qu’il envoie des messages électroniques sans dépasser les limites de l' [expéditeur Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Par exemple, utilisez une pause dans le flux de travail, envoyez le courrier électronique à un groupe Office 365, à un groupe de distribution ou à un groupe de sécurité à extension messagerie, ou envoyez le message à un nombre de destinataires inférieur à 200 à la fois.


Pour plus d’informations, consultez l' [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)suivant.

## <a name="related-topics"></a>Sujets associés
- [Créer un flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint et flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 