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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080744"
---
# <a name="create-an-email-catch-all"></a>Créer un e-mail catch all

L’utilisation d’un « catch all » est fortement déconseillée. Il est préférable de renvoyer un message à l’expéditeur pour lui faire savoir que son message n’a pas pu être remis comme traité afin qu’il puisse prendre des mesures. Vous pouvez également limiter la boîte aux lettres surveillée pour qu’elle capture uniquement les adresses de messagerie auparavant valides. 

Toute boîte aux lettres « catch » reçoit une grande partie du courrier indésirable et peut finir par remplir si elle n’est pas surveillée de près. (Il existe des limites de réception.) 

Si vous décidez de continuer, procédez comme suit :

1. Créez un groupe de distribution dynamique & « Tous les types de destinataires ».

2. Créez une boîte aux lettres dédiée pour capturer les messages électroniques, par exemple, catchall@domain.com.

3. Pour le domaine spécifique, définissez DomainType sur « InternalRelay ». Si vous supprimez ultérieurement le catch all, assurez-vous de définir le domaine sur Faisant autorité.

4. Créez une règle de transport de flux de messagerie comme suit :

    - Si l’expéditeur est « en dehors de l’organisation »
    - Rediriger le message vers Catchall@domain.com
    - Sauf si le destinataire est membre de allusers@domain.com (le groupe de distribution contient tous les membres)
    - Vérifier que les nouvelles boîtes aux lettres sont ajoutées au groupe de distribution dynamique
