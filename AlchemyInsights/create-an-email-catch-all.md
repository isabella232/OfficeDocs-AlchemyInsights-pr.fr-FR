---
title: Créer un e-mail catch all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816198"
---
# <a name="create-an-email-catch-all"></a>Créer un e-mail catch all

L’utilisation d’un « catch all » est fortement déconseillée. Il est préférable de renvoyer une nouvelle fois à l’expéditeur pour que les expéditeurs sachent que leur message n’a pas pu être remis comme traité afin qu’ils prennent des mesures. Vous pouvez également limiter la boîte aux lettres surveillée pour qu’elle capture uniquement les adresses de messagerie auparavant valides. 

Toute boîte aux lettres « catch » reçoit une grande partie du courrier indésirable et peut finir par remplir si elle n’est pas surveillée de près. (Il existe des limites de réception.) 

Si vous décidez de continuer, procédez comme suit :

1. Créez un groupe de distribution dynamique & inclure « Tous les types de destinataires ».

2. Créez une boîte aux lettres dédiée pour capturer les messages électroniques, par exemple, catchall@domain.com.

3. Pour le domaine spécifique, définissez DomainType sur « InternalRelay ». Si vous supprimez ultérieurement le catch all, n’oubliez pas de définir le domaine sur Faisant autorité.

4. Créez une règle de transport de flux de messagerie comme suit :

    - Si l’expéditeur est « en dehors de l’organisation »
    - Rediriger le message vers Catchall@domain.com
    - Sauf si le destinataire est membre de allusers@domain.com (le groupe de distribution contient tous les membres)
    - Vérifier que les nouvelles boîtes aux lettres sont ajoutées au groupe de distribution dynamique
