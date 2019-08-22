---
title: Identifier l’activité des règles de boîte de réception dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539164"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifier l’activité des règles de boîte de réception dans les journaux d’audit

Vous pouvez utiliser la recherche dans le journal d’audit dans le centre de sécurité & de la sécurité Office 365 pour afficher les événements de règles de boîte de réception (création, modification et suppression de règles de boîte de réception).

1. Connectez-vous au [Centre de sécurité & conformité Office 365](https://protection.office.com/).

2. Accédez à la page de**recherche du journal d’audit** de la **recherche** > .

3. Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** .

4. Sous **activités de boîte aux lettres Exchange**, vérifiez que le champ **activités** est défini sur **nouveau-InboxRule créer/modifier/activer/désactiver la règle de boîte de réception**.

5. Cliquez sur **Rechercher**.

Dans les résultats, sélectionnez un enregistrement d’audit. Dans la fenêtre mobile des détails, cliquez sur **informations supplémentaires**. Les informations sur les paramètres des règles de boîte de réception sont affichées dans le champ **paramètres** .

Pour plus d’informations, consultez [la rubrique déterminer si un utilisateur a créé une règle de boîte de réception](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
