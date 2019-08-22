---
title: Identifier les événements de suppression de messages dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539207"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Journaux d’audit pour les messages électroniques supprimés

À compter du 1er janvier 2019, Microsoft Active la journalisation d’audit des boîtes aux lettres par défaut. Dans le cas contraire, pour examiner les événements de suppression de message pour un utilisateur spécifique, vous devez activer manuellement les actions de suppression pour l’audit. Si la journalisation d’audit des boîtes aux lettres est déjà activée pour votre organisation ou pour un utilisateur spécifique, suivez les étapes ci-dessous.

1. Connectez-vous au [Centre de conformité & Office 365 Security](https://protection.office.com/)

2. Cliquez sur **recherche et enquête** , puis sélectionnez **recherche du journal d’audit**.

3. Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** . Spécifiez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner (l’utilisateur qui a supprimé les éléments). Dans le champ **activités** , sélectionnez **messages supprimés du dossier éléments supprimés** et **messages déplacés dans le dossier éléments supprimés**.

4. Cliquez sur **Rechercher**.

Dans les résultats, sélectionnez un enregistrement d’audit. Dans la fenêtre mobile des détails, cliquez sur **informations supplémentaires**. Des informations supplémentaires sur l’élément supprimé (par exemple, la ligne d’objet et l’emplacement de l’élément lors de sa suppression) s’affichent dans le champ **AffectedItems** . La propriété **ClientInfoString** indique si la suppression s’est produite dans Outlook, Outlook sur le Web (anciennement appelé Outlook Web App) ou un autre appareil.

Pour plus d’informations, consultez [la rubrique Détermination de la personne qui a configuré le transfert du courrier pour une boîte aux lettres](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Remarque**: vous ne pouvez pas récupérer les éléments supprimés à l’aide de la fonctionnalité de journal d’audit. Pour récupérer des messages supprimés dans Outlook sur le Web, consultez la rubrique [récupérer des éléments supprimés dans Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
