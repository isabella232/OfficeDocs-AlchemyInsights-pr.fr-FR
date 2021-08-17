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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058648"
---
# <a name="find-events-performed-on-inbox-rules"></a>Rechercher des événements effectués sur des règles de boîte de réception

Lorsque des règles de boîte de réception sont créées, modifiées ou supprimées, les événements sont enregistrés dans le journal d’audit. Voici comment les examiner :

1. Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Sélectionnez Rechercher > recherche dans le journal d’audit.

    > [!NOTE]
    > Si un avis vous demande d’activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.
1. Sélectionnez le champ Activités et recherchez Exchange activités de boîte aux lettres, puis sélectionnez New-InboxRule créer une règle de boîte de réception à partir Outlook Web App. Lorsque vous avez terminé, cliquez en dehors du volet pour réduire le volet Activités.
1. Spécifiez la plage de dates, puis dans le champ Utilisateurs, sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner. Vous pouvez sélectionner plusieurs utilisateurs à la fois.
1. Sélectionner Rechercher. Les activités s’affichent sous Résultats.
1. Pour afficher les détails, sélectionnez une activité, puis sélectionnez Plus d’informations. Sous la section Paramètres, vous pouvez voir le nom de la règle, les conditions définies et les actions que la règle va prendre.

Pour en savoir plus, consultez la Office 365 d’audit pour résoudre les problèmes courants.