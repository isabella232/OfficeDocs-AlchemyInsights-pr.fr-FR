---
title: Identifier les événements de message de suppression dans les journaux d’audit
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630067"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Journaux d’audit pour les messages électroniques supprimés

À compter de janvier 2019, Microsoft démarre l’enregistrement d’audit des boîtes aux lettres par défaut. Dans le cas contraire, pour passer en revue les événements de message de suppression pour un utilisateur spécifique, vous devez activer manuellement les actions de suppression pour l’audit. Si l’enregistrement d’audit de boîte aux lettres est déjà activé pour votre organisation ou pour l’utilisateur spécifique, suivez les étapes ci-dessous.

1. Connectez-vous au [Centre Microsoft 365 conformité de l’application](https://protection.office.com/)

2. Cliquez **sur Recherche et enquête,** puis sélectionnez Recherche dans le journal **d’audit.**

3. Sélectionnez la plage de dates dans les champs **Date de** début et **Date de** fin. Spécifiez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner (l’utilisateur qui a supprimé les éléments). Dans le **champ Activités,** sélectionnez Messages supprimés du dossier **Éléments** supprimés et Messages déplacés vers le dossier **Éléments supprimés.**

4. Cliquez sur **Rechercher**.

Dans les résultats, sélectionnez un enregistrement d’audit. Dans le volant de détails, cliquez sur **Plus d’informations.** Des informations supplémentaires sur l’élément supprimé (par exemple, la ligne d’objet et l’emplacement de l’élément lors de sa suppression) s’affichent dans le champ **AffectedItems.** La **propriété ClientInfoString** indique si la suppression s’est produite dans Outlook, Outlook sur le web (anciennement Outlook Web App) ou tout autre appareil.

Pour plus d’informations, voir Déterminer qui a installé le forwarding de courrier [pour une boîte aux lettres.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Remarque**: vous ne pouvez pas récupérer les éléments supprimés à l’aide de la fonctionnalité journal d’audit. Pour récupérer des messages supprimés dans Outlook sur le web, voir Récupérer les éléments supprimés [dans Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
