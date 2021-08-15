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
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976863"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifier l’activité des règles de boîte de réception dans les journaux d’audit

Vous pouvez utiliser la recherche dans le journal d’audit dans le Centre de sécurité & conformité Microsoft 365 pour afficher les événements de règle de boîte de réception (création, modification et suppression de règles de boîte de réception).

1. Connectez-vous au [Centre Microsoft 365 conformité.](https://protection.office.com/)

2. Go to the **Search**  >  **Audit log search** page.

3. Sélectionnez la plage de dates dans les champs **Date de** début et **Date de** fin.

4. Sous **Exchange activités** de boîte aux  lettres, vérifiez que le champ Activités est définie sur Nouvelle boîte de réception **Créer/modifier/activer/désactiver la** règle de boîte de réception .

5. Cliquez sur **Rechercher**.

Dans les résultats, sélectionnez un enregistrement d’audit. Dans le volant de détails, cliquez sur **Plus d’informations.** Les informations sur les paramètres de règle de boîte de réception sont affichées dans **le champ Paramètres.**

Pour plus d’informations, voir [Déterminer si un utilisateur a créé une règle de boîte de réception](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
