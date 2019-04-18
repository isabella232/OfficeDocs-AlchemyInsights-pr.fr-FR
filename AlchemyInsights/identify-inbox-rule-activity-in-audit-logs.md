---
title: Identifier l'activité des règles de boîte de réception dans les journaux d'audit
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909222"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifier l'activité des règles de boîte de réception dans les journaux d'audit

Vous pouvez utiliser la recherche de journal d'audit dans le centre de sécurité & Compliance Center pour afficher les événements de règles de boîte de réception (création, modification et suppression de règles de boîte de réception).

1. Connectez-vous au [Centre de sécurité & de sécurité Office 365](https://protection.office.com/)

2. Cliquez sur **recherche et enquête** , puis sélectionnez **recherche du journal d'audit**.

3. Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** .

4. Sous **activités de boîte aux lettres Exchange**, vérifiez que le champ **activités** est défini sur **nouveau-InboxRule créer/modifier/activer/désactiver la règle de boîte de réception**.

5. Cliquez sur **Rechercher**.

Dans les résultats, sélectionnez un enregistrement d'audit. Dans la fenêtre mobile des détails, cliquez sur **informations supplémentaires**. Les informations sur les paramètres des règles de boîte de réception sont affichées dans le champ **paramètres** .

Pour plus d'informations, consultez [la rubrique déterminer si un utilisateur a créé une règle de boîte de réception](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
