---
title: Rechercher des événements effectués sur des règles de boîte de réception
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464702"
---
# <a name="find-events-performed-on-inbox-rules"></a>Rechercher des événements effectués sur des règles de boîte de réception

Lorsque des règles de boîte de réception sont créées, modifiées ou supprimées, les événements sont enregistrés dans le journal d’audit. Voici comment les examiner :

1. Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Sélectionnez Rechercher > recherche dans le journal d’audit.

    > [!NOTE]
    > Si un avis vous demande d’activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.
1. Sélectionnez le champ Activités et recherchez les activités de boîte aux lettres Exchange, puis sélectionnez New-InboxRule créer une règle de boîte de réception à partir d’Outlook Web App. Lorsque vous avez terminé, cliquez en dehors du volet pour réduire le volet Activités.
1. Spécifiez la plage de dates, puis dans le champ Utilisateurs, sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner. Vous pouvez sélectionner plusieurs utilisateurs à la fois.
1. Sélectionnez Rechercher. Les activités apparaissent sous Résultats.
1. Pour afficher les détails, sélectionnez une activité, puis sélectionnez Plus d’informations. Sous la section Paramètres, vous pouvez voir le nom de la règle, les conditions définies et les actions que la règle va prendre.

Pour en savoir plus, consultez la recherche dans le journal d’audit Office 365 pour résoudre les problèmes de scénarios courants.