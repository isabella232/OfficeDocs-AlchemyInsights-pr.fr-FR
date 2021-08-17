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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313497"
---
# <a name="find-events-performed-on-inbox-rules"></a>Rechercher des événements effectués sur des règles de boîte de réception

Lorsque des règles de boîte de réception sont créées, modifiées ou supprimées, les événements sont enregistrés dans le journal d’audit. Voici comment les examiner :

1. Faites l’une des actions suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://security.microsoft.com/auditlogsearch> .

    **Remarque**: si vous voyez une notification vous avisant que vous devez activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.
1. Sélectionnez le champ Activités et recherchez Exchange activités de boîte aux lettres, puis sélectionnez créer New-InboxRule boîte de réception à partir Outlook Web App. Lorsque vous avez terminé, cliquez en dehors du volet pour réduire le volet Activités.
1. Spécifiez la plage de dates, puis dans le champ Utilisateurs, sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner. Vous pouvez sélectionner plusieurs utilisateurs à la fois.
1. Sélectionner Rechercher. Les activités s’affichent sous Résultats.
1. Pour afficher les détails, sélectionnez une activité, puis sélectionnez Plus d’informations. Sous la section Paramètres, vous pouvez voir le nom de la règle, les conditions définies et les actions que la règle va prendre.

2. Sous **l’onglet** Recherche de la page **Audit,** configurez les paramètres suivants :
   - **Date et plage de dates :** sélectionnez la plage date/heure dans les zones Début **et** Fin. 
   - **Activités :** sélectionner **une règle de boîte** de réception Créer une boîte de réception à partir Outlook Web App

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.**

4. Sélectionnez une activité dans les résultats pour ouvrir le volant de détails. Sous la section **Paramètres,** vous pouvez voir le nom de la règle, les conditions définies et les actions que la règle va prendre.

Pour en savoir plus, [consultez la recherche dans le journal d’audit pour examiner les problèmes de support courants.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
