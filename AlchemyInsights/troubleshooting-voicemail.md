---
title: 'Dépannage de la messagerie vocale '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607998"
---
# <a name="troubleshooting-voicemail"></a>Dépannage de la messagerie vocale

Assurez-vous que la fonctionnalité Busy on Busy est intentionnelle.

Si cette fonctionnalité n’est pas nécessaire sur cet utilisateur :

1. Accédez au [Centre d’administration teams](https://admin.teams.microsoft.com/policies/calling).
1. Sur le rail gauche, naviguez vers les  >  **stratégies d’appel** vocal  >  **gérer les stratégies** sur la stratégie d' **appel**.
1. Sélectionnez **gérer les utilisateurs**.
1. Recherchez utilisateur et modifiez la stratégie d’appel de façon à ce qu’elle **soit disponible lorsqu’elle est en cours** d' appel.
1. Cliquez sur **Appliquer**.
> [!NOTE]
> La réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.

Pour plus d’informations sur cette fonctionnalité, reportez-vous à la rubrique : [Busy on Busy est disponible lors d’un appel](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
