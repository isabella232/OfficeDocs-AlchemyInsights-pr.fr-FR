---
title: 618 Stratégie de partage de calendrier
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091601"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erreur de stratégie lors du partage d’un calendrier

1. Faites l’une des choses suivantes, selon votre situation :
    - Connecter à Exchange Online à l’aide de Remote PowerShell. Pour plus d’informations, [voir Connecter à Exchange Online à l’aide de Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Sur le serveur local, ouvrez l’Exchange Management Shell.
2. Déterminez la stratégie de partage attribuée à l’utilisateur. Pour ce faire, exécutez la commande suivante et notez la stratégie renvoyée :

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Mettez à jour la stratégie de partage pour l’utilisateur. Pour cela, procédez comme suit :
    - Ouvrez le Centre d’administration Exchange.
    - Cliquez **sur** Organisation, puis double-cliquez sur la stratégie attribuée à l’utilisateur sous **Partage individuel.** Il s’agit de la stratégie renvoyée à l’étape 2.
    - Dans la page Règle de partage, sélectionnez le niveau de partage de calendrier que vous souhaitez autoriser sous Spécifier les **informations que vous souhaitez partager**. cliquez **sur Enregistrer.**

Pour plus d’informations, voir : « La stratégie n’autorise pas l’octroi d’autorisations à ce niveau à un ou plusieurs des destinataires » lorsque l’utilisateur tente de [partager le calendrier.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
