---
title: Identifier l’activité des règles de boîte de réception dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331121"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifier l’activité des règles de boîte de réception dans les journaux d’audit

Vous pouvez utiliser la recherche dans le journal d’audit dans le Centre de conformité Microsoft 365 pour afficher les événements de règle de boîte de réception (création, modification et suppression de règles de boîte de réception).

1. Effectuez l’une des étapes suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://security.microsoft.com/auditlogsearch> .

2. Sous **l’onglet** Recherche de la page **Audit,** configurez les paramètres suivants :
   - **Date et plage de dates :** sélectionnez la plage date/heure dans les zones Début **et** Fin. 
   - **Activités :** sélectionnez une ou plusieurs des valeurs suivantes :
     - **Règle de boîte de réception Créer une boîte de réception New-InboxRule à partir Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Mettre à jour les règles de boîte de réception Outlook client**

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.**

4. Sélectionnez une activité dans les résultats pour ouvrir le volant de détails. Les informations sur les paramètres de règle de boîte de réception sont affichées dans **le champ Paramètres.**

Pour plus d’informations, voir [Déterminer si un utilisateur a créé une règle de boîte de réception.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
