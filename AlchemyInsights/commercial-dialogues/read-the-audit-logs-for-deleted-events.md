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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896013"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Lire les journaux d’audit pour les événements supprimés

Voici comment faire :

1. Faites l’une des actions suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Si vous voyez une notification vous avisant que vous devez activer la fonctionnalité, allez de l’avant et l’activer maintenant. Si la fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.

2. Sous **l’onglet** Recherche de la page **Audit,** configurez les paramètres suivants :
   - **Date et plage de dates :** sélectionnez la plage date/heure dans les zones Début **et** Fin. 
   - **Activités : entrez** Exchange **activités de boîte aux** lettres, puis sélectionnez les valeurs suivantes :
     - **Messages supprimés du dossier Éléments supprimés**
     - **Messages déplacés vers le dossier Éléments supprimés**

       Lorsque vous avez terminé, cliquez en dehors du volet pour réduire le **volet** Activités.

   - **Utilisateurs**: acceptez la valeur par défaut vide pour renvoyer des résultats pour tous les utilisateurs, ou entrez un ou plusieurs utilisateurs.

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.**

4. Sélectionnez une activité dans les résultats pour ouvrir le volant de détails. Des informations supplémentaires sur l’élément supprimé, telles que la ligne d’objet et l’emplacement de l’élément lors de sa suppression, sont affichées dans le champ **AffectedItems.**

   > [!NOTE]
   > Vous ne pouvez pas restaurer les éléments supprimés à l’aide de la fonctionnalité journal d’audit. Pour restaurer les éléments supprimés, voir [Récupérer les messages électroniques](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)supprimés dans Outlook sur le web .

Pour plus d’informations, [consultez la recherche dans le journal d’audit pour examiner les problèmes de support courants.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
