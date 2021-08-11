---
title: Lire les journaux d’audit pour les événements supprimés
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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967331"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Lire les journaux d’audit pour les événements supprimés

Voici comment faire :

1. Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Sélectionnez **recherche**  >  [**dans le journal d’audit de recherche.**](https://go.microsoft.com/fwlink/?linkid=2103759)
    > [!NOTE]
    > Si vous voyez une notification vous avisant que vous devez activer la fonctionnalité, allez de l’avant et l’activer maintenant. Si la fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.
1. Sélectionnez **Activités,** puis recherchez Exchange **activités de boîte aux lettres.** Sélectionnez **les messages supprimés** du dossier Éléments supprimés et les **options du** dossier Éléments supprimés. Lorsque vous avez terminé, cliquez en dehors du volet pour réduire **le** volet Activités.
1. Spécifiez la plage de dates, puis dans la zone **Utilisateurs,** sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner. Vous pouvez sélectionner plusieurs utilisateurs à la fois.
1. Sélectionner **Rechercher**. Les activités s’affichent sous **Résultats**.
1. Pour afficher les détails, sélectionnez une activité, puis sélectionnez **Plus d’informations.** Des informations supplémentaires sur l’élément supprimé, telles que la ligne d’objet et l’emplacement de l’élément lors de sa suppression, sont affichées dans le champ **AffectedItems.**
    > [!NOTE]
    > Vous ne pouvez pas restaurer les éléments supprimés à l’aide de la fonctionnalité journal d’audit. Pour restaurer des éléments supprimés, voir Récupérer les éléments supprimés ou le [courrier électronique dans Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)

Pour plus d’informations, consultez la Office 365 [d’audit pour résoudre les problèmes courants.](https://go.microsoft.com/fwlink/?linkid=2103944)
