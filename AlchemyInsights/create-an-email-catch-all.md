---
title: Créer un e-mail attraper tout
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286108"
---
# <a name="create-an-email-catch-all"></a>Créer un e-mail attraper tout

L’utilisation d’une capture tout est fortement déconseillée. Il est préférable de renvoyer un message à l’expéditeur pour informer les expéditeurs qu’ils n’ont pas pu être remis comme adressés afin qu’ils puissent agir. Vous pouvez également limiter la boîte aux lettres surveillée afin d’intercepter uniquement les adresses de messagerie valides précédemment. 

Toute boîte aux lettres peut recevoir une grande quantité de courrier indésirable et éventuellement remplir si elle n’est pas soigneusement surveillée. (Il existe des limites de réception.) 

Si vous décidez de procéder, procédez comme suit :

1. Créez un groupe de distribution dynamique & inclure « tous les types de destinataires ».

2. Créez une boîte aux lettres dédiée pour intercepter des courriers électroniques, par exemple, catchall@domain.com.

3. Pour le domaine spécifique, définissez DomainType sur « InternalRelay ». Si vous supprimez par la suite le paramètre catch tout, veillez à redéfinir le domaine sur faisant autorité.

4. Créez une règle de transport de flux de flux comme suit :

    - Si l’expéditeur est « à l’extérieur de l’Organisation »
    - Rediriger le message vers Catchall@domain.com
    - Sauf si le destinataire est membre de allusers@domain.com (le groupe de distribution contient tous les membres)
    - Vérifier que les nouvelles boîtes aux lettres sont ajoutées au groupe de distribution dynamique
