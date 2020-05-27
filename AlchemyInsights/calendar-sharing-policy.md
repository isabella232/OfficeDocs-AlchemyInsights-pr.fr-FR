---
title: Stratégie de partage de calendrier 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372997"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erreur de stratégie lors du partage d’un calendrier

1. Effectuez l’une des opérations suivantes, selon votre situation :
    - Connectez-vous à Exchange Online à l’aide de PowerShell à distance. Pour plus d’informations, consultez la rubrique [connexion à Exchange Online à l’aide de Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Sur le serveur local, ouvrez l’environnement de commande Exchange Management Shell.
2. Déterminer la stratégie de partage qui est attribuée à l’utilisateur. Pour ce faire, exécutez la commande suivante et notez la stratégie renvoyée :

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Mettez à jour la stratégie de partage pour l’utilisateur. Pour cela, procédez comme suit:
    - Ouvrez le Centre d’administration Exchange.
    - Cliquez sur **organisation**, puis double-cliquez sur la stratégie qui est attribuée à l’utilisateur sous **partage individuel**. Il s’agit de la stratégie qui a été renvoyée à l’étape 2.
    - Dans la page règle de partage, sélectionnez le niveau de partage de calendrier que vous souhaitez autoriser sous **Spécifiez les informations que vous souhaitez partager**; Cliquez sur **Enregistrer**.

Pour plus d’informations, voir : ["la stratégie n’autorise pas l’octroi d’autorisations à ce niveau à un ou plusieurs destinataires" lorsque l’utilisateur tente de partager le calendrier](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
